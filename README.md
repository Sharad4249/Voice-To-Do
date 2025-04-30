# Voice Todo App

A Flutter-based todo app that lets users manage tasks using voice commands. The app supports offline mode with voice command queueing and syncs across devices in real-time.

## Features

- 🎤 Voice Command Support
  - Add tasks: "Add buy groceries"
  - Complete tasks: "Complete buy groceries"
  - Delete tasks: "Delete meeting note"

- 📦 Offline Support
  - Works without internet connection
  - Queues voice commands for later sync
  - Local storage using Hive

- 🔄 Real-time Sync
  - Syncs across multiple devices
  - Uses Firebase Firestore
  - Automatic conflict resolution

- 🔊 Voice Feedback
  - Audible confirmation of actions
  - Error notifications
  - Command status updates

## Setup

1. Install Flutter dependencies:
   ```bash
   flutter pub get
   ```

2. Configure Firebase:
   - Create a new Firebase project
   - Add your Android/iOS apps
   - Download and replace the Firebase configuration in `lib/firebase_options.dart`
   - Enable Firestore in your Firebase Console

3. Run the app:
   ```bash
   flutter run
   ```

## Dependencies

- **State Management**: flutter_riverpod
- **Database**: 
  - Local: Hive
  - Cloud: Firebase Firestore
- **Voice Processing**:
  - Speech to Text: speech_to_text
  - Text to Speech: flutter_tts
- **Utilities**:
  - connectivity_plus
  - uuid
  - intl

## Architecture

The app follows a clean architecture pattern:

- `models/`: Data models
- `providers/`: State management
- `services/`: Business logic
- `screens/`: UI components

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request 