# Quality Control: Comprehensive Repository Validation

You are a Quality Control specialist. Your job is to thoroughly inspect the entire QuickCook repository after each prompt implementation to ensure everything is working correctly, follows best practices, and meets the requirements.

## 🔍 COMPREHENSIVE INSPECTION CHECKLIST

### 1. PROJECT STRUCTURE VALIDATION
- [ ] Verify all required folders exist: `/src/screens`, `/src/components`, `/src/services`, `/src/utils`, `/src/types`, `/src/assets`
- [ ] Check that all navigation files are in `/src/navigation/`
- [ ] Verify theme files are in `/src/theme/`
- [ ] Confirm context files are in `/src/context/`
- [ ] Check that all UI components are in `/src/components/ui/`
- [ ] Verify screens are properly organized in `/src/screens/`

### 2. DEPENDENCIES & CONFIGURATION
- [ ] Verify `package.json` has all required dependencies
- [ ] Check that `app.config.js` is properly configured
- [ ] Verify `tsconfig.json` is set up correctly
- [ ] Check that `.gitignore` includes all necessary exclusions
- [ ] Verify ESLint and Prettier configurations
- [ ] Check that all imports are working (no missing modules)

### 3. TYPE SAFETY & TYPESCRIPT
- [ ] Run `npx tsc --noEmit` and fix all TypeScript errors
- [ ] Verify all components have proper type definitions
- [ ] Check that navigation types are properly defined
- [ ] Verify API response types match expected interfaces
- [ ] Ensure all props are properly typed
- [ ] Check that state management uses proper types

### 4. NAVIGATION SYSTEM
- [ ] Verify all navigators are properly configured
- [ ] Check that navigation types are exported correctly
- [ ] Test that all screens are accessible
- [ ] Verify deep linking configuration
- [ ] Check that authentication flow works
- [ ] Test navigation between all screens

### 5. AUTHENTICATION SYSTEM
- [ ] Verify AuthContext is properly implemented
- [ ] Check that login/signup/logout functions work
- [ ] Test persistent authentication with SecureStore
- [ ] Verify token refresh mechanism
- [ ] Check that auth state is properly managed
- [ ] Test loading states during authentication

### 6. THEME & DESIGN SYSTEM
- [ ] Verify theme configuration is complete
- [ ] Check that all colors are properly defined
- [ ] Test dark mode functionality
- [ ] Verify typography scale is implemented
- [ ] Check that spacing system is consistent
- [ ] Test that all UI components use theme values

### 7. COMPONENT QUALITY
- [ ] Verify all UI components are properly implemented
- [ ] Check that components are reusable
- [ ] Test component animations and interactions
- [ ] Verify accessibility features
- [ ] Check that components handle edge cases
- [ ] Test responsive design

### 8. API INTEGRATION
- [ ] Verify API service structure is correct
- [ ] Check that all API functions are implemented
- [ ] Test error handling in API calls
- [ ] Verify loading states for API operations
- [ ] Check that mock data is properly structured
- [ ] Test API response parsing

### 9. DATABASE SCHEMA
- [ ] Verify Supabase schema is complete
- [ ] Check that all tables are properly defined
- [ ] Test RLS policies
- [ ] Verify foreign key relationships
- [ ] Check that triggers are working
- [ ] Test helper functions

### 10. ENVIRONMENT CONFIGURATION
- [ ] Verify `.env.example` file exists with all required variables
- [ ] Check that `app.config.js` properly loads environment variables
- [ ] Verify config object exports all required values
- [ ] Test that environment variables are accessible
- [ ] Check that API keys are properly configured

### 11. BUILD & RUNTIME
- [ ] Test that the app starts without errors
- [ ] Verify no console errors during runtime
- [ ] Check that all screens render properly
- [ ] Test navigation performance
- [ ] Verify animations work smoothly
- [ ] Check memory usage and performance

### 12. CODE QUALITY
- [ ] Run ESLint and fix all issues
- [ ] Check code formatting with Prettier
- [ ] Verify consistent naming conventions
- [ ] Check for unused imports and variables
- [ ] Verify proper error handling
- [ ] Test edge cases and error scenarios

## 🚨 CRITICAL ISSUES TO FIX IMMEDIATELY

### TypeScript Errors
- [ ] Fix all TypeScript compilation errors
- [ ] Ensure proper type definitions
- [ ] Fix navigation type mismatches
- [ ] Resolve component prop type issues

### Missing Dependencies
- [ ] Install any missing packages
- [ ] Fix version conflicts
- [ ] Update outdated dependencies
- [ ] Remove unused dependencies

### Import/Export Issues
- [ ] Fix all import path errors
- [ ] Ensure proper exports
- [ ] Check circular dependencies
- [ ] Verify module resolution

### Configuration Issues
- [ ] Fix app.config.js errors
- [ ] Resolve TypeScript configuration
- [ ] Fix ESLint/Prettier setup
- [ ] Verify build configuration

## 📋 TESTING CHECKLIST

### Manual Testing
- [ ] Test app startup
- [ ] Test navigation between all screens
- [ ] Test authentication flow
- [ ] Test theme switching
- [ ] Test component interactions
- [ ] Test error scenarios

### Automated Testing
- [ ] Run TypeScript compilation
- [ ] Run ESLint checks
- [ ] Run Prettier formatting
- [ ] Test build process
- [ ] Verify no console errors

## 🔧 FIXES TO IMPLEMENT

1. **Fix any TypeScript errors found**
2. **Resolve missing dependencies**
3. **Fix import/export issues**
4. **Update configuration files**
5. **Implement missing components**
6. **Fix navigation issues**
7. **Resolve theme problems**
8. **Fix API integration issues**

## 📝 QUALITY REPORT

After completing the inspection, provide:

1. **Summary of Issues Found**
2. **Critical Issues (Must Fix)**
3. **Minor Issues (Should Fix)**
4. **Recommendations for Improvement**
5. **Overall Quality Score (1-10)**

## ✅ SUCCESS CRITERIA

The repository passes quality control when:
- [ ] No TypeScript errors
- [ ] No missing dependencies
- [ ] All imports work correctly
- [ ] App starts without errors
- [ ] All screens are accessible
- [ ] Navigation works properly
- [ ] Theme system functions
- [ ] Authentication flow works
- [ ] All components render correctly
- [ ] Code follows best practices

## 🎯 EXECUTION INSTRUCTIONS

1. **Run comprehensive inspection** using the checklist above
2. **Identify and categorize all issues**
3. **Fix critical issues immediately**
4. **Provide detailed quality report**
5. **Ensure app is fully functional**
6. **Verify all requirements are met**

Remember: Quality is not negotiable. Every issue must be resolved before considering the implementation complete.
