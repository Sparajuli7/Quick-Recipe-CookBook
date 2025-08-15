# Prompt 07: State Management Setup

Implement global state management using Zustand:
1.
Install zustand and zustand/middleware
2.
Create /src/store/ folder with slices:
3.
authStore.ts:
 - user object
 - isAuthenticated boolean
 - isPremium boolean
 - login/logout/updateProfile actions
 - Persist auth state to SecureStore
4.
recipeStore.ts:
 - currentRecipe
 - savedRecipes array (max 10 for free)
 - recipesGeneratedToday counter
 - addSavedRecipe/removeSavedRecipe actions
 - Daily reset logic for recipe generation count
5.
ingredientStore.ts:
 - availableIngredients array
 - addIngredient/removeIngredient actions
 - clearAll action
 - Voice input temporary storage
6.
mealPlanStore.ts:
 - weeklyMealPlan object
 - shoppingList array
 - addMealToDay/removeMealFromDay actions
 - generateShoppingList action
7.
uiStore.ts:
 - isDarkMode boolean
 - isLoading states for different operations
 - activeFilters object
 - showOnboarding boolean
 - Error/success message queue
8.
Create store hooks:
 - useAuth()
 - useRecipes()
 - useIngredients()
 - useMealPlan()
 - useUI()

## ✅ Verify Success:
- [Verification steps will be added based on the specific prompt]
