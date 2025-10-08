# ShopEZ Mobile Shopping App

**ShopEZ** is a mobile shopping application built with React Native and Firebase. It allows users to register, log in, browse products from the Fake Store API, filter them by category, and manage a personal shopping cart.

## Features ✨

-   **User Authentication**: Secure sign-up and login with Firebase Authentication (Email/Password).
-   **Persistent Login**: Users stay logged in across app restarts.
-   **Product Catalog**: Fetches and displays products from the [Fake Store API](https://fakestoreapi.com/).
-   **Category Filtering**: Filter products by category.
-   **Product Details**: View detailed information for each product.
-   **Shopping Cart**: Add/remove items and update quantities. The cart is saved to Firebase Realtime Database and is unique to each user.
-   **Offline Persistence**: The user's cart is saved locally using AsyncStorage, so it's visible even without an internet connection.
-   **React Navigation**: A clean, stack-based navigation flow between screens.

## Setup and Installation 🚀

Follow these steps to get the project running on your local machine.

### 1. Prerequisites

-   [Node.js](https://nodejs.org/) (LTS version recommended)
-   [Expo Go](https://expo.dev/client) app on your iOS or Android device.

### 2. Clone the Repository

```bash
git clone <your-repository-url>
cd ShopEZ
```

### 3. Install Dependencies

Install the necessary packages using npm or yarn.

```bash
npm install
```

### 4. Configure Firebase 🔥

This project requires a Firebase project to handle authentication and the database.

1.  Go to the [Firebase Console](https://console.firebase.google.com/) and create a new project.
2.  In your new project, go to **Project settings** and create a new **Web App**.
3.  You will be given a `firebaseConfig` object. Copy these credentials.
4.  Open the `firebaseConfig.js` file in the root of this project.
5.  Replace the placeholder configuration object with your own credentials.
6.  In the Firebase Console, navigate to the **Authentication** section, click the **Sign-in method** tab, and enable the **Email/Password** provider.
7.  Navigate to the **Realtime Database** section and create a new database. Start in **test mode** for easy setup.

### 5. Run the Application

Once the dependencies are installed and Firebase is configured, you can start the development server.

```bash
npx expo start
```

This will open a Metro Bundler window in your browser. Scan the QR code with the Expo Go app on your phone to run the application.
