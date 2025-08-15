# Prompt 18: Recipe Generation & Results

Create AI-powered recipe generation and results display:
1.
Create /src/services/recipeGenerator.ts:
 - Build structured prompt for GPT
 - Include ingredients, dietary filters, cooking time
 - Request JSON format with specific schema
 - Use GPT-3.5 for free users, GPT-4 for premium
2.
Prompt engineering template:
Generate 5 recipes using ONLY these ingredients: [ingredients]
Dietary requirements: [filters]
Format as JSON array with: title, cookingTime, difficulty, servings, ingredients (with amounts), instructions (step array), nutrition
Make recipes varied in cuisine and cooking method
3.
Create /src/screens/main/RecipeResultsScreen.tsx:
 - Loading state with cooking puns
 - Grid layout for recipe cards (2 columns)
 - Each card shows: * Recipe image (AI-generated or stock) * Title * Cooking time chip * Difficulty indicator * Diet tags * Start Cooking button
4.
Recipe card interactions:
 - Press to expand with more details
 - Save button (bookmark icon)
 - Share button
 - Nutrition preview
5.
Filtering and sorting:
 - Sort by time, difficulty
 - Filter by cuisine type
 - Hide recipes with missing ingredients
 - Premium filters (calories, protein, etc.)
6.
Error states:
 - No recipes found
 - Suggest removing filters
 - Try different ingredients
 - API error handling

## ✅ Verify Success:
- [Verification steps will be added based on the specific prompt]
