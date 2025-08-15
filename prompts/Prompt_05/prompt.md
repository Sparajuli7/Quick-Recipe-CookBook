# Prompt 05: Navigation Structure

Set up complete navigation structure with authentication flow:
1.
Create navigation structure in /src/navigation/:
 - AuthNavigator.tsx: Login, Signup, ForgotPassword screens
 - MainNavigator.tsx: Bottom tabs with Home, Saved, Meal Plan, Profile
 - RootNavigator.tsx: Switches between Auth and Main based on auth state
2.
Implement bottom tab navigation with:
 - Custom tab bar with glassmorphism effect
 - Animated active tab indicator
 - Icons: Home (chef hat), Saved (bookmark), Plan (calendar), Profile (user)
 - Badge for saved recipes count (max 10 for free users)
3.
Create stack navigators within each tab:
 - Home Stack: Home → Recipe Details → Cooking Mode
 - Saved Stack: Saved Recipes → Recipe Details
 - Plan Stack: Meal Planner → Shopping List
 - Profile Stack: Profile → Settings → Subscription
4.
Add authentication state management:
 - AuthContext.tsx with login/logout/signup methods
 - Persistent authentication using SecureStore
 - Auto-refresh tokens
 - Loading state while checking auth
5.
Implement deep linking for:
 - Recipe sharing: quickcook://recipe/[id]
 - Meal plans: quickcook://plan/[date]
 - Premium upgrade: quickcook://upgrade

## ✅ Verify Success:
- [Verification steps will be added based on the specific prompt]
