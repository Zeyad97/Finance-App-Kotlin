# 💰 Kotlin Finance App

<div align="center">

[![Kotlin](https://img.shields.io/badge/kotlin-%237F52FF.svg?style=for-the-badge&logo=kotlin&logoColor=white)](https://kotlinlang.org/)
[![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com/)
[![Firebase](https://img.shields.io/badge/firebase-%23039BE5.svg?style=for-the-badge&logo=firebase)](https://firebase.google.com/)
[![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white)](https://developer.android.com/jetpack/compose)

**A modern, feature-rich Android finance application built with Kotlin and Jetpack Compose**

[Features](#-features) • [Architecture](#-architecture) • [Installation](#-installation) • [Documentation](#-documentation) • [Screenshots](#-screenshots)

</div>

## 📱 Overview

The **Kotlin Finance App** is a comprehensive personal finance management application designed to help users track their income, expenses, and financial goals. Built with modern Android development practices, it features a clean Material Design 3 interface, real-time data synchronization, and robust user authentication.

### 🎯 Key Highlights

- **100% Kotlin** - Modern, safe, and concise code
- **Jetpack Compose UI** - Declarative, responsive user interface
- **Firebase Integration** - Real-time data sync and authentication
- **MVVM Architecture** - Clean, testable, and maintainable code structure
- **Material Design 3** - Beautiful, accessible user experience
- **Comprehensive Documentation** - Every line of code explained in detail

## ✨ Features

### 🔐 Authentication & Security
- **User Registration & Login** - Secure Firebase Authentication
- **Profile Management** - User profile with display name customization
- **Session Management** - Automatic login/logout handling
- **Data Privacy** - User-specific data isolation

### 💸 Transaction Management
- **Add Transactions** - Quick income and expense entry
- **Edit & Delete** - Full CRUD operations for transactions
- **Categories** - Pre-defined and custom transaction categories
- **Real-time Updates** - Instant UI updates with data changes

### 📊 Financial Dashboard
- **Balance Overview** - Current financial status at a glance
- **Income/Expense Summary** - Visual breakdown with color-coded indicators
- **Transaction History** - Chronological list of all transactions
- **Financial Insights** - Quick balance calculations and trends

### ⚙️ Settings & Customization
- **Theme Selection** - Dark and light mode support
- **Currency Support** - Multiple international currencies
- **Export Data** - CSV export for external analysis
- **User Preferences** - Persistent settings storage

### 📈 Data Export
- **CSV Export** - Export transactions to CSV format
- **Email Sharing** - Share financial data via email
- **Cloud Backup** - Automatic Firebase cloud storage

## 🏗️ Architecture

This application follows **Clean Architecture** principles with **MVVM pattern**:

### 📁 Project Structure
```
app/
├── data/                          # Data layer
│   ├── FirebaseAuthRepository     # Authentication implementation
│   ├── FirebaseTransactionRepository # Transaction data management
│   ├── PreferencesManager        # User preferences storage
│   └── Models (Transaction, User, Category)
├── ui/screens/                    # Presentation layer
│   ├── HomeScreen                 # Dashboard interface
│   ├── LoginScreen                # Authentication UI
│   ├── AddTransactionScreen       # Transaction entry
│   └── SettingsScreen             # App configuration
├── viewmodel/                     # Business logic layer
│   ├── FinanceViewModel           # Financial operations
│   └── AuthViewModel              # Authentication state
└── MainActivity                   # App entry point & navigation
```

### 🔧 Tech Stack

| Component | Technology |
|-----------|------------|
| **Language** | Kotlin |
| **UI Framework** | Jetpack Compose |
| **Architecture** | MVVM + Repository Pattern |
| **Backend** | Firebase (Auth + Firestore) |
| **Navigation** | Compose Navigation |
| **State Management** | StateFlow + Compose State |
| **Dependency Injection** | Manual DI |
| **Persistence** | SharedPreferences + Firestore |

## 🚀 Installation

### Prerequisites
- Android Studio Arctic Fox or newer
- Android SDK 24+ (Android 7.0)
- Firebase account for backend services

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/Zeyad97/Finance-App-Kotlin.git
   cd Finance-App-Kotlin
   ```

2. **Open in Android Studio**
   - Launch Android Studio
   - Select "Open an existing project"
   - Navigate to the cloned directory

3. **Configure Firebase**
   - Create a new Firebase project at [Firebase Console](https://console.firebase.google.com/)
   - Add an Android app to your project
   - Download `google-services.json` and place it in `app/` directory
   - Enable Authentication (Email/Password) and Firestore Database

4. **Build and Run**
   ```bash
   ./gradlew assembleDebug
   ```
   Or use Android Studio's run button

## 📚 Documentation

This project includes **comprehensive documentation** for every component:

### 📖 Available Documentation
- **[COMPLETE_DOCUMENTATION.md](COMPLETE_DOCUMENTATION.md)** - Complete technical documentation for developers
- **[CLIENT_TECHNICAL_DOCUMENTATION.txt](CLIENT_TECHNICAL_DOCUMENTATION.txt)** - Business-friendly project overview
- **Inline Code Comments** - Every line of code explained in detail

### 🔍 Code Documentation Features
- **Line-by-line explanations** for all functions and classes
- **Architecture decisions** and design patterns explained
- **Firebase integration** step-by-step breakdown
- **UI component** detailed documentation
- **Business logic** comprehensive explanations

## 📱 Screenshots

<div align="center">

| Login Screen | Dashboard | Add Transaction | Settings |
|:------------:|:---------:|:---------------:|:--------:|
| ![Login](docs/screenshots/login.png) | ![Dashboard](docs/screenshots/dashboard.png) | ![Add Transaction](docs/screenshots/add.png) | ![Settings](docs/screenshots/settings.png) |

*Clean, modern interface with Material Design 3*

</div>

## 🛠️ Development

### 🏃‍♂️ Running the App
```bash
# Debug build
./gradlew assembleDebug

# Release build
./gradlew assembleRelease

# Run tests
./gradlew test
```

### 📝 Code Style
- **Kotlin Coding Conventions** - Following official Kotlin style guide
- **Material Design 3** - Modern UI components and theming
- **Clean Architecture** - Separation of concerns and testability

### 🧪 Testing
- Unit tests for ViewModels and business logic
- UI tests for critical user flows
- Firebase rules testing for data security

### 📋 Development Guidelines
1. Follow the existing code style and architecture
2. Add comprehensive documentation for new features
3. Include unit tests for business logic
4. Update README if adding new features

## 👨‍💻 Author

**Zeyad97**
- GitHub: [@Zeyad97](https://github.com/Zeyad97)

## 🙏 Acknowledgments

- **Firebase** for providing robust backend services
- **Android Jetpack** for modern development tools
- **Material Design** for beautiful UI components
- **Kotlin** for making Android development enjoyable

