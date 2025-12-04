# Flash Chat Flutter

A modern, lightweight messaging application built with **Flutter** and powered by **Firebase**. This app demonstrates real-time messaging capabilities, secure user authentication, and fluid animations.

## Features

* **Real-time Messaging:** Instant chat updates using Cloud Firestore.
* **User Authentication:** Secure sign-up and login functionality via Firebase Auth.
* **Hero Animations:** Smooth transitions between welcome, login, and registration screens.
* **Modern UI:** Clean interface with distinct message bubbles for senders and receivers.
* **Typewriter Effect:** engaging text animations on the welcome screen.

## Screenshots

| Welcome Screen | Login Screen | Chat Screen |
|:---:|:---:|:---:|
| <img src="demo/flash_chat_flutter_demo.gif.png" width="200"> 
## Tech Stack

* **Framework:** [Flutter](https://flutter.dev/) (Dart)
* **Backend:** [Firebase](https://firebase.google.com/)
    * **Authentication:** For user management.
    * **Cloud Firestore:** NoSQL database for real-time data storage.
* **Packages:**
    * `firebase_core`
    * `firebase_auth`
    * `cloud_firestore`
    * `animated_text_kit` (for text animations)
    * `modal_progress_hud_nsn` (for loading spinners)

## Getting Started

Follow these steps to get a copy of the project running on your local machine.

### Prerequisites

* [Flutter SDK](https://flutter.dev/docs/get-started/install) installed.
* An IDE (VS Code or Android Studio).
* A Firebase account.

### Installation

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/otolis/FlashChatFlutter.git](https://github.com/otolis/FlashChatFlutter.git)
    cd FlashChatFlutter/flash_chat
    ```

2.  **Install Dependencies:**
    ```bash
    flutter pub get
    ```

3.  **Firebase Setup (Crucial Step):**
    * Go to the [Firebase Console](https://console.firebase.google.com/).
    * Create a new project.
    * **Android:** Register an Android app (using the package name from `android/app/build.gradle`) and download the `google-services.json` file. Place it in `android/app/`.
    * **iOS:** Register an iOS app and download the `GoogleService-Info.plist`. Place it in `ios/Runner/`.
    * Enable **Authentication** (Email/Password method) in the Firebase console.
    * Create a **Cloud Firestore** database and set the security rules to allow read/write (for testing purposes).

4.  **Run the App:**
    ```bash
    flutter run
    ```

