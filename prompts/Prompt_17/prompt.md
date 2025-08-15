# Prompt 17: Barcode Scanner

Implement barcode scanning for ingredients:
1.
Install and configure:
 - expo-barcode-scanner
 - Camera permissions handling
 - Spoonacular API for barcode lookup
2.
Create /src/screens/main/BarcodeScannerScreen.tsx:
 - Full-screen camera view
 - Scanning frame overlay
 - Torch/flashlight toggle
 - Close button to return
3.
Scanning interface:
 - Auto-focus on barcode
 - Beep sound on successful scan
 - Vibration feedback
 - Show product preview card
4.
Product lookup flow:
 - Call Spoonacular barcode API
 - Show loading state
 - Display product name and image
 - Extract main ingredient
 - Add to ingredients list button
5.
Multi-scan mode:
 - Keep scanning after each item
 - Show running list of scanned items
 - Bulk add all items button
 - Clear all button
6.
Error handling:
 - Product not found message
 - Network error handling
 - Manual ingredient entry fallback
 - Try again button
7.
UI Polish:
 - Animated scan line
 - Brightness boost in dark environments
 - History of recent scans
 - Tips for better scanning

## ✅ Verify Success:
- [Verification steps will be added based on the specific prompt]
