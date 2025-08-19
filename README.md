# SuperFind 🦸‍♂️

A SwiftUI-based iOS application for searching and managing favorite superhero information, developed as part of a Mobile Applications for iPhone course.

## 📱 Features

### Hero Search 🔍
- **Real-time Search**: Search for superheroes by name using an intuitive search interface
- **API Integration**: Fetches hero data from the SuperHero API
- **Hero List Display**: Shows search results with hero image, name, alias, and favorite button
- **Detailed Navigation**: Tap any hero to view complete information

### Hero Details 🦸
- **Complete Information**: Displays detailed hero stats including strength, intelligence, speed, and power
- **Biographical Data**: Shows place of birth, alignment, and other character details
- **High-Quality Images**: Large hero images for better visual experience
- **Favorite Management**: Add or remove heroes from favorites directly from detail view

### Favorites Management ❤️
- **Local Storage**: Persistent storage using Core Data for offline access
- **Favorites Collection**: Dedicated view to browse saved favorite heroes
- **Quick Actions**: Easy removal of heroes from favorites
- **Data Persistence**: Favorites survive app restarts and device reboots

## 🏗️ Architecture

The project follows a clean architecture pattern with clear separation of concerns:
SuperFind/
├── Data/              # Data layer - API & Core Data
├── Domain/            # Business logic & models  
├── Presentation/      # UI layer - Views & ViewModels
└── Assets.xcassets/   # App resources & icons

### Key Components

- **Data Layer**: 
  - `HeroService.swift` - API communication
  - `FavoriteDAO.swift` - Core Data operations
  - `PersistenceController.swift` - Core Data stack management
  - `HeroDTO.swift` - Data transfer objects

- **Domain Layer**:
  - `Hero.swift` - Hero business model
  - `Favorite.swift` - Favorite entity model

- **Presentation Layer**:
  - **Views**: SwiftUI views for each screen
  - **ViewModels**: Business logic for view states
  - `UIState.swift` - Application state management

## 🛠️ Technical Stack

- **Language**: Swift
- **UI Framework**: SwiftUI
- **Data Persistence**: Core Data
- **Architecture**: MVVM (Model-View-ViewModel)
- **API**: [SuperHero API](https://superheroapi.com/)
- **iOS Version**: iOS 14.0+

## 🚀 Getting Started

### Prerequisites
- Xcode 12.0 or later
- iOS 14.0+ deployment target
- Active internet connection for hero search

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/andrea-13-12/SuperFind.git

2. Open SuperFind.xcodeproj in Xcode
3. Build and run the project on simulator or device

### API Configuration
The app uses the SuperHero API with the following endpoint:
https://superheroapi.com/api/f274286a22873ec9fc7a5782940f7ca2/search/{name}

# 📱 Screenshots
Add screenshots of your app here

# 🎯 Project Requirements Met
This project successfully implements all required features:
✅ Navigation: Fluid navigation between multiple screens
✅ UI Layout: Adaptive design for different screen sizes
✅ State Management: Proper view state handling
✅ Web Services: Dynamic data consumption from API
✅ Local Persistence: Core Data implementation for favorites
✅ SwiftUI: Built exclusively with SwiftUI framework

### 📁 Project Structure
SuperFind/
├── SuperFindApp.swift          # App entry point
├── ContentView.swift           # Main content view
├── Data/
│   ├── HeroService.swift       # API service
│   ├── FavoriteDAO.swift       # Core Data operations
│   ├── HeroDTO.swift           # Data models
│   ├── HeroModel.xcdatamodeld  # Core Data model
│   └── PersistenceController.swift
├── Domain/
│   ├── Hero.swift              # Hero domain model
│   └── Favorite.swift          # Favorite entity
└── Presentation/
    ├── UIState.swift           # UI state management
    ├── View/
    │   ├── FindHeroView.swift
    │   ├── HeroDetailView.swift
    │   ├── FavoriteListView.swift
    │   ├── HeroListItemView.swift
    │   └── FavoriteListItemView.swift
    └── ViewModel/
        ├── FindHeroViewModel.swift
        └── FavoriteListViewModel.swift

### 🔧 Key Features Implementation
# Search Functionality

- Text input field with real-time search capability
- API integration with error handling
- Loading states and user feedback

# Hero Details

- Comprehensive hero information display
- Statistics visualization
- Biographical information presentation

# Favorites System
- Core Data persistence
- Add/remove favorite operations
- Offline data access

# 🎓 Academic Project
This application was developed as part of the Mobile Applications for iPhone course (2025-10), demonstrating:

- iOS development best practices
- SwiftUI framework proficiency
- Core Data implementation
- API integration
- Clean architecture principles

### 📄 License
This project is for educational purposes as part of university coursework.

### 👨‍💻 Author
Developed by Andrea Torres Cerdan as part of iOS Development coursework.

Feel free to explore the code and provide feedback! This project showcases fundamental iOS development concepts including SwiftUI, Core Data, and API integration.
