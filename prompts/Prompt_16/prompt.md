# Prompt 16: Voice Input Integration

Implement voice input using OpenAI Whisper:
1.
Install and configure:
 - expo-av for audio recording
 - Set up Whisper API integration
 - Request microphone permissions
2.
Create /src/components/VoiceInput.tsx:
 - Microphone button with hold-to-record
 - Visual wave animation while recording
 - "Listening..." text display
 - Auto-stop after 30 seconds
3.
Voice processing logic:
 - Record audio in proper format for Whisper
 - Send to OpenAI Whisper API
 - Parse transcription for ingredients
 - Handle multiple ingredients in one phrase
 - Support phrases like "I have chicken, rice, and broccoli"
4.
Natural language processing:
 - Extract quantities ("2 pounds of chicken")
 - Handle variations ("tomatoes" vs "tomato")
 - Ignore filler words
 - Support multiple languages (optional)
5.
Feedback and confirmation:
 - Show transcription before adding
 - Allow editing transcribed text
 - Confidence indicator for recognition
 - Error messages for unclear audio
6.
Polish:
 - Haptic feedback on start/stop
 - Cancel recording gesture
 - Background noise handling
 - Voice coaching tips

## ✅ Verify Success:
- [Verification steps will be added based on the specific prompt]
