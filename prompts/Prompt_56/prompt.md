# Prompt 56: Form Validation & Input Handling

Implement comprehensive form validation and input handling for data integrity:

## 1. Zod Validation Schemas
Create /src/validation/schemas.ts:
- User registration schema
- Recipe creation schema
- Ingredient input schema
- Meal plan schema
- Profile update schema
- Search query schema

## 2. Form Validation Hooks
Create /src/hooks/useFormValidation.ts:
- Real-time validation
- Field-level error handling
- Validation state management
- Custom validation rules
- Cross-field validation

## 3. Input Components
Create /src/components/forms/:
- ValidatedInput.tsx: Base input with validation
- ValidatedTextArea.tsx: Text area with validation
- ValidatedSelect.tsx: Select with validation
- ValidatedCheckbox.tsx: Checkbox with validation
- ValidatedDatePicker.tsx: Date picker with validation

## 4. Error Display System
Create /src/components/forms/FormError.tsx:
- Field-specific error messages
- Error message styling
- Error animation effects
- Accessibility for screen readers
- Error clearing on input

## 5. Form State Management
Create /src/utils/formState.ts:
- Form state persistence
- Dirty state tracking
- Form submission handling
- Validation state caching
- Form reset functionality

## 6. Input Sanitization
Create /src/utils/inputSanitizer.ts:
- XSS prevention
- SQL injection prevention
- Input length limits
- Special character handling
- Data type validation

## 7. Accessibility Features
Ensure forms are:
- Keyboard navigable
- Screen reader compatible
- Error message accessible
- Focus management
- ARIA labels and descriptions

## 8. Validation Rules
Implement validation for:
- Email format and uniqueness
- Password strength requirements
- Required field validation
- Data type validation
- Business logic validation

## ✅ Verify Success:
- [ ] All forms validate correctly
- [ ] Error messages are clear
- [ ] Forms are accessible
- [ ] Input sanitization works
- [ ] Validation prevents invalid data
