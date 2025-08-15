# Prompt 55: Loading States & Skeleton Screens

Implement comprehensive loading states and skeleton screens for optimal user experience:

## 1. Skeleton Screen Components
Create /src/components/skeletons/:
- RecipeCardSkeleton.tsx: Recipe card loading state
- HomeScreenSkeleton.tsx: Home screen loading
- ProfileSkeleton.tsx: Profile loading state
- SearchSkeleton.tsx: Search results loading
- MealPlanSkeleton.tsx: Meal planner loading

## 2. Loading State Management
Create /src/hooks/useLoadingState.ts:
- Global loading state management
- Loading state for specific operations
- Loading state persistence
- Loading state transitions
- Loading state analytics

## 3. Progressive Loading
Implement progressive loading for:
- Recipe images with blur-up effect
- List items with virtual scrolling
- Large datasets with pagination
- Heavy components with lazy loading
- Background data prefetching

## 4. Loading Animations
Create /src/components/animations/:
- PulseAnimation.tsx: Pulsing loading effect
- ShimmerAnimation.tsx: Shimmer loading effect
- SpinnerAnimation.tsx: Custom spinner
- ProgressBar.tsx: Progress indicators
- SkeletonWave.tsx: Wave loading effect

## 5. Context-Aware Loading
Implement loading states for:
- API calls and data fetching
- Image loading and caching
- Form submissions
- Navigation transitions
- Background sync operations

## 6. Loading State Optimization
Optimize loading experience:
- Preload critical data
- Cache loading states
- Minimize loading time
- Provide loading feedback
- Handle loading failures

## 7. Accessibility for Loading
Ensure loading states are:
- Screen reader accessible
- Keyboard navigable
- High contrast compatible
- Reduced motion friendly
- Clear and informative

## ✅ Verify Success:
- [ ] All async operations show loading states
- [ ] Skeleton screens look realistic
- [ ] Loading animations are smooth
- [ ] No blank screens during loading
- [ ] Loading states are accessible
