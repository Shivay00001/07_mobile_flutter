# 07_mobile_flutter - Offline-First Mobile App

> Production-grade Flutter application demonstrating offline-first architecture and cross-platform development.

## 🎯 Overview

This module implements:

- **Offline-First** - Local-first data sync
- **Clean Architecture** - Layered design
- **State Management** - Riverpod/BLoC
- **Native Features** - Camera, Location, Biometrics

## 📁 Structure

```
07_mobile_flutter/
├── lib/
│   ├── core/                # Core utilities
│   │   ├── di/              # Dependency injection
│   │   ├── network/         # API client
│   │   └── storage/         # Local storage
│   ├── features/            # Feature modules
│   │   ├── auth/            # Authentication
│   │   ├── orders/          # Order management
│   │   └── inventory/       # Inventory scanning
│   └── main.dart            # Entry point
├── test/                    # Tests
└── pubspec.yaml             # Dependencies
```

## 🚀 Quick Start

```bash
# Get dependencies
flutter pub get

# Run on device/emulator
flutter run

# Build for release
flutter build apk --release
flutter build ios --release
```

## 🏗️ Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    PRESENTATION                             │
│          Widgets │ Pages │ State Management                 │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                      DOMAIN                                 │
│           Use Cases │ Entities │ Repositories               │
└─────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────┐
│                       DATA                                  │
│      Remote │ Local │ Sync │ Data Sources                  │
└─────────────────────────────────────────────────────────────┘
```

## 📄 License

MIT
