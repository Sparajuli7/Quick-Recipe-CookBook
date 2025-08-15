# Prompt 13: Social Authentication

Implement Google and Apple Sign In:
1.
Configure Google Sign In:
 - Install expo-auth-session and expo-web-browser
 - Set up Google Cloud Console OAuth 2.0
 - Configure for iOS, Android, and Web
 - Add proper redirect URIs
2.
Configure Apple Sign In:
 - Install expo-apple-authentication
 - Configure in Apple Developer Console
 - Set up Sign in with Apple capability
 - Handle iOS-only availability
3.
Create /src/services/socialAuth.ts:
 - googleSignIn() method
 - appleSignIn() method
 - Link social accounts to Supabase
 - Handle profile data extraction
 - Profile picture handling
4.
Update login/signup screens:
 - Add social login buttons
 - "Continue with Google" button
 - "Sign in with Apple" button (iOS only)
 - Loading states for social auth
5.
Handle edge cases:
 - Account already exists with email
 - Social login cancelled
 - Network errors during OAuth
 - Profile data missing

## ✅ Verify Success:
- [Verification steps will be added based on the specific prompt]
