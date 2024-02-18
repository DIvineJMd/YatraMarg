# Journey Tracker App (Yatraमार्ग)

## Overview
The Journey Tracker app is designed to provide users with information about their journey, including details about stops, distances between stops, and the overall progress of the journey. The app offers a user-friendly interface with the ability to switch between kilometers and miles, mark stops as reached, and visualize the journey's progress.

## Features
- **Unit Switching:** Users can toggle between displaying distances in kilometers and miles by using a dedicated button.
- **Stop Marking:** A button allows users to indicate that they have reached the next stop in their journey.
- **Progress Visualization:** The app includes a progress section that displays each stop, their distances, the total distance covered, and the remaining distance. A progress bar visually represents the journey's progress.
- **Lazy List:** For journeys with more than 10 stops, the app utilizes a lazy list to efficiently handle large datasets.
- **Compatibility:** The app is designed to run seamlessly on both Android devices and the Android emulator.

## Getting Started
To run the Journey Tracker app on your Android device or emulator, follow these steps:
1. Clone the repository to your local machine.
git clone https://github.com/DIvineJMd/YatraMarg.git
2. Open the project in Android Studio.
3. Run the app on your desired device or emulator.

## Technologies Used
- **Kotlin:** The programming language used for app development.
- **Android Compose:** A modern UI toolkit for building native Android UI.

## Code Structure
### MainActivity.kt
This is an Android application built with Jetpack Compose and Navigation Compose.

#### MainActivity
The `MainActivity` is the entry point of the application. It sets up the navigation for the app using `NavHost` and `rememberNavController`.

#### Navigation
The app has two screens: `Home` and `Second`. The `NavHost` is set up with these two routes. The `startDestination` is set to `Home`, which means the app will open with the `Home` screen.

#### Home Screen
The `Home` screen is represented by the `JHome().homeScreen(navController)` composable function. This function takes in the `NavController` as a parameter, which is used for navigating between different screens.

#### Second Screen
The `Second` screen is represented by the `secondScreen(navController)` composable function. This function also takes in the `NavController` as a parameter.

#### Theme
The app uses a custom theme defined in `LearndAppTheme`. The `Surface` composable is used to apply this theme to the entire app.

#### StatusBarColor
The status bar color is set to white using the `Setcolorbar().SetStatusBarColor(color = Color.White)` function.

#### Preview
The `DefaultPreview` function is a preview function that can be used to preview composables in Android Studio.

### 2. JHome.kt
