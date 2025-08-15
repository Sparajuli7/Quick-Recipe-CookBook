# Prompt 06: API Service Layer

Create comprehensive API service layer for all external services:
1.
Create /src/services/api/ folder with:
2.
openai.service.ts:
 - generateRecipe(ingredients, filters, useGPT4)
 - Structured prompt engineering for consistent JSON responses
 - Token counting and cost estimation
 - Error handling and retry logic
 - Response validation with Zod schemas
3.
spoonacular.service.ts:
 - searchByBarcode(upc)
 - getIngredientInfo(ingredient)
 - getNutritionData(recipe)
 - autocompleteIngredient(query)
 - Error handling for API limits
4.
supabase.service.ts:
 - Authentication methods (login, signup, logout, resetPassword)
 - Profile CRUD operations
 - Recipe CRUD operations
 - Meal plan management
 - Real-time subscriptions setup
5.
stripe.service.ts:
 - createCustomer(email)
 - createSubscription(customerId, priceId)
 - cancelSubscription(subscriptionId)
 - handleWebhook(event)
 - Payment method management
6.
cache.service.ts:
 - In-memory cache with TTL
 - Recipe cache management
 - Ingredient cache
 - Cache invalidation strategies
7.
analytics.service.ts:
 - Track events to both Mixpanel and Amplitude
 - User property updates
 - Revenue tracking
 - Funnel analysis events

## ✅ Verify Success:
- [Verification steps will be added based on the specific prompt]
