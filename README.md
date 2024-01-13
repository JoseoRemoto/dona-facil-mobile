# DonaFacilMobile
The Mobile application of Dona Facil is developed using Flutter, allowing for a cross-platform experience across iOS and Android. This app integrates with the Dona Facil backend to offer users the full range of features, including account management, item listings, and community interactions, all from their mobile devices.

# 

### **Overview**

Dona Facil's mobile app is designed to provide a convenient and accessible way for users to engage with the platform. Key aspects include:

- **Cross-Platform Compatibility**: Developed in Flutter for use on both iOS and Android.
- **User-Friendly Interface**: Focused on delivering an intuitive user experience.
- **Offline Capabilities**: Includes features like offline data caching for enhanced performance.
- **Push Notifications**: For real-time alerts and updates to the users.

Technologies used:

- Framework: Flutter.
- State Management: Provider, Bloc, or any other state management technique preferred.
- API Integration: HTTP package for RESTful API communication.

### **2. Getting Started**

### Prerequisites

Make sure you have the following installed:

- Flutter (latest stable version)
- Dart SDK
- An IDE like Android Studio, VSCode, or IntelliJ

### **3. App Architecture**

The architecture of the Dona Facil mobile app is designed to ensure scalability, maintainability, and efficiency. We adopt a clean architecture approach with Flutter, focusing on modularization, testability, and separation of concerns.

### Key Architectural Components:

1. **Model-View-ViewModel (MVVM)**:
    - We use the MVVM pattern to separate the UI logic from the business logic.
    - **Models**: Represent the data structure and business logic.
    - **Views**: UI components/screens that display the data.
    - **ViewModels**: Act as a bridge between Models and Views, handling the presentation logic.
2. **State Management**:
    - **Provider Package**: Used for state management across the app. It helps in efficiently updating UI when the underlying data changes.
    - **Stream Controllers**: For reactive data handling, particularly useful for real-time features.
3. **Routing and Navigation**:
    - Utilizing Flutter's Navigator 2.0 for advanced routing capabilities.
    - Defined routes and a centralized navigation management system for handling transitions between screens.
4. **API Integration**:
    - **HTTP Client**: For RESTful API communication with the backend.
    - Implementation of a repository pattern to abstract the data layer, making it scalable and independent of the data source.
5. **Database and Local Storage**:
    - **SQLite**: For local database storage to cache data and manage offline data.
    - **Shared Preferences**: For storing simple data persistently across sessions (like user settings).
6. **Dependency Injection**:
    - Using packages like **`get_it`** for dependency injection, ensuring a decoupled and testable codebase.
7. **Testing**:
    - Unit Tests: For testing individual functions and classes.
    - Widget Tests: To test individual widgets.
    - Integration Tests: To test complete workflows.
8. **Continuous Integration/Continuous Deployment (CI/CD)**:
    - Implementation of CI/CD pipelines for automated testing and deployment.
9. **Folder Structure**:
    - **lib/**: Contains the Dart source files.
        - **models/**: Data models.
        - **views/**: UI screens or widgets.
        - **viewmodels/**: ViewModels for business logic.
        - **services/**: Services like API communication, database access.
        - **utils/**: Utility classes and functions.
        - **constants/**: Constant values used throughout the app.

By adhering to this architecture, the Dona Facil mobile app ensures a robust, maintainable, and scalable application, capable of handling the dynamic needs of the users while providing a seamless user experience.
