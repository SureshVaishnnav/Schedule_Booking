# Schedule Booking Application

A smart scheduling application built with Flutter that helps users balance work, personal development, and relaxation while ensuring productivity and well-being.

## 🎯 Features

- 📅 Smart Schedule Management
  - Create and organize events
  - Recurring schedules
  - Time slot management
  - Conflict detection

- ⚖️ Work-Life Balance
  - Category-based scheduling
  - Priority management
  - Break reminders
  - Wellness tracking

- 🔔 Intelligent Notifications
  - Custom reminders
  - Smart alerts
  - Quiet hours support
  - Push notifications

- 📊 Analytics & Insights
  - Productivity tracking
  - Time analysis
  - Goal progress
  - Weekly reports

- 🎨 User-Friendly Interface
  - Intuitive calendar view
  - Drag-and-drop scheduling
  - Dark mode support
  - Responsive design

## 🛠️ Technologies Used

- Flutter
- Dart
- Firebase (Backend & Authentication)
- Local Storage
- GetX (State Management)
- Provider (State Management)

## 📋 Prerequisites

- Flutter SDK 3.0+
- Dart 3.0+
- Android Studio or Xcode
- Firebase account

## 🚀 Getting Started

```bash
# Clone repository
git clone https://github.com/SureshVaishnnav/Schedule_Booking.git

# Install dependencies
cd Schedule_Booking
flutter pub get

# Setup Firebase
# Update google-services.json (Android)
# Update GoogleService-Info.plist (iOS)

# Run the app
flutter run

# Build for production
flutter build apk      # Android
flutter build ios      # iOS
```

## 📁 Project Structure

```
lib/
├── screens/
│   ├── home/
│   ├── schedule/
│   ├── analytics/
│   └── settings/
├── widgets/
├── models/
├── services/
├── controllers/
├── utils/
└── main.dart
```

## 🔧 Configuration

### Firebase Setup

1. Create Firebase project
2. Add Android app:
   - Download `google-services.json`
   - Place in `android/app/`
3. Add iOS app:
   - Download `GoogleService-Info.plist`
   - Place in `ios/Runner/`

### Environment Variables

Create `lib/config/env.dart`:

```dart
class Env {
  static const String firebaseApiKey = 'your_api_key';
  static const String firebaseAuthDomain = 'your_auth_domain';
  // ... other config
}
```

## 💡 Usage

### Creating a Schedule

```dart
class ScheduleCreation {
  final String title;
  final DateTime startTime;
  final DateTime endTime;
  final String category; // work, personal, rest
  final String priority; // high, medium, low
  final bool recurring;
  
  ScheduleCreation({
    required this.title,
    required this.startTime,
    required this.endTime,
    required this.category,
    this.priority = 'medium',
    this.recurring = false,
  });
}
```

### Schedule Categories

- **Work**: Tasks and meetings
- **Personal Development**: Learning and skill building
- **Relaxation**: Rest and wellness
- **Health**: Exercise and nutrition
- **Social**: Family and friends

## 📊 Analytics Features

- Daily productivity score
- Category-wise time distribution
- Schedule completion rate
- Weekly/Monthly reports
- Progress visualization

## 🔔 Smart Notifications

- Task reminders
- Break notifications
- Deadline alerts
- Schedule conflicts
- Wellness reminders

## 🎨 Customization

### Themes

```dart
class AppTheme {
  static ThemeData lightTheme() {
    return ThemeData(
      brightness: Brightness.light,
      primaryColor: Colors.blue,
      // ... more customization
    );
  }
  
  static ThemeData darkTheme() {
    return ThemeData(
      brightness: Brightness.dark,
      primaryColor: Colors.blue,
      // ... more customization
    );
  }
}
```

## 📱 Supported Platforms

- Android 5.0+ (API 21+)
- iOS 11.0+
- Web (Flutter Web)

## 🧪 Testing

```bash
# Run unit tests
flutter test

# Run with coverage
flutter test --coverage

# Run integration tests
flutter drive --target=test_driver/app.dart
```

## 🔐 Security Features

- Firebase Authentication
- Secure data storage
- Encrypted local data
- Privacy-first design

## 🚀 Performance Optimization

- Lazy loading
- Image caching
- Efficient state management
- Optimized database queries
- Memory management

## 📝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 🐛 Known Issues & Roadmap

- [ ] Cloud sync across devices
- [ ] Team scheduling
- [ ] Integration with calendar apps
- [ ] AI-powered scheduling suggestions
- [ ] Video call integration
- [ ] Expense tracking

## 📚 Resources

- [Flutter Documentation](https://flutter.dev/docs)
- [Firebase for Flutter](https://firebase.flutter.dev/)
- [Dart Programming](https://dart.dev/guides)

## 📄 License

MIT License

---

**Made with ❤️ by Suresh Vaishnav**
