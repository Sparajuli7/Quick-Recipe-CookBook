# Prompt 03: Supabase Database Schema

Create complete Supabase database schema and authentication setup:

1. Create Supabase project and configure authentication:
   - Enable email/password authentication
   - Enable Google OAuth
   - Enable Apple Sign In (for iOS)
   - Set up magic link authentication

2. Create database tables:

```sql
-- Users table (extends Supabase auth.users)
CREATE TABLE profiles (
  id UUID REFERENCES auth.users PRIMARY KEY,
  username TEXT UNIQUE,
  full_name TEXT,
  avatar_url TEXT,
  is_premium BOOLEAN DEFAULT false,
  premium_expires_at TIMESTAMP,
  stripe_customer_id TEXT,
  recipes_generated_today INTEGER DEFAULT 0,
  last_recipe_reset_at DATE DEFAULT CURRENT_DATE,
  onboarding_completed BOOLEAN DEFAULT false,
  dietary_preferences JSONB DEFAULT '[]',
  created_at TIMESTAMP DEFAULT NOW(),
  updated_at TIMESTAMP DEFAULT NOW()
);

-- Recipes table
CREATE TABLE recipes (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  title TEXT NOT NULL,
  ingredients JSONB NOT NULL,
  instructions JSONB NOT NULL,
  cooking_time INTEGER,
  difficulty TEXT CHECK (difficulty IN ('easy', 'medium', 'hard')),
  servings INTEGER DEFAULT 4,
  nutrition JSONB,
  image_url TEXT,
  tags TEXT[],
  ai_model TEXT,
  created_by UUID REFERENCES profiles(id),
  is_public BOOLEAN DEFAULT false,
  created_at TIMESTAMP DEFAULT NOW()
);

-- Saved recipes
CREATE TABLE saved_recipes (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  user_id UUID REFERENCES profiles(id) ON DELETE CASCADE,
  recipe_id UUID REFERENCES recipes(id) ON DELETE CASCADE,
  notes TEXT,
  rating INTEGER CHECK (rating >= 1 AND rating <= 5),
  cooked_count INTEGER DEFAULT 0,
  last_cooked_at TIMESTAMP,
  created_at TIMESTAMP DEFAULT NOW(),
  UNIQUE(user_id, recipe_id)
);

-- Meal plans
CREATE TABLE meal_plans (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  user_id UUID REFERENCES profiles(id) ON DELETE CASCADE,
  week_start_date DATE NOT NULL,
  meals JSONB NOT NULL,
  shopping_list JSONB,
  created_at TIMESTAMP DEFAULT NOW(),
  updated_at TIMESTAMP DEFAULT NOW()
);

-- Recipe cache for cost optimization
CREATE TABLE recipe_cache (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  ingredient_hash TEXT UNIQUE NOT NULL,
  recipes JSONB NOT NULL,
  hit_count INTEGER DEFAULT 1,
  created_at TIMESTAMP DEFAULT NOW(),
  last_accessed_at TIMESTAMP DEFAULT NOW()
);

-- Analytics events
CREATE TABLE analytics_events (
  id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
  user_id UUID REFERENCES profiles(id),
  event_name TEXT NOT NULL,
  event_data JSONB,
  created_at TIMESTAMP DEFAULT NOW()
);
```

3. Set up Row Level Security (RLS) policies for all tables
4. Create database triggers for updated_at timestamps
5. Set up Supabase Storage buckets for recipe images
6. Create helper functions and stored procedures

## ✅ Verify Success:
- All tables created in Supabase dashboard
- RLS policies enabled and tested
- Can insert test data via Supabase UI
