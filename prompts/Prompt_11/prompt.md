# Prompt 11: Forgot Password Screen

Create a simple forgot password flow:
1.
Create /src/screens/auth/ForgotPasswordScreen.tsx:
 - Clean glass card design
 - Email input field
 - Clear instructions text
 - Send reset link button
 - Back to login link
2.
Implement password reset flow:
 - Validate email format
 - Call Supabase resetPassword
 - Show success message
 - Countdown timer (60s) before resend
 - Check email instructions
3.
Add animations:
 - Slide in from right
 - Success envelope animation
 - Loading state for sending
4.
Handle edge cases:
 - Email not found (don't reveal for security)
 - Too many reset attempts
 - Network errors
 - Expired reset links

## ✅ Verify Success:
- [Verification steps will be added based on the specific prompt]
