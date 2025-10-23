# 🗺️ Personal Map Application

https://i.ibb.co/WN3JwmQy/Screenshot-20251023-200616-Chrome.jpg

This project is a single-page web application that serves as a personalized map where authenticated users can save specific locations, track their real-time location, search for saved places, calculate routes, and even draw and save custom routes. It utilizes **Leaflet.js** for interactive mapping and **Firebase** for a complete backend solution (Authentication and Realtime Database).

## ✨ Features

* **User Authentication:** Secure login and registration using Firebase Authentication (Email/Password).
* **Real-time Location Tracking:** Track and display your live GPS location and accuracy circle on the map.
* **Saved Places (Markers):**
    * Add custom markers to the map by clicking a location.
    * Save places with a custom name to the Firebase Realtime Database.
    * Double-click a marker to prompt for deletion.
* **Place Search:** Search for saved places with auto-suggestions.
* **Routing:**
    * **Path:** Calculate the shortest driving route between your live location and a saved place using Leaflet Routing Machine.
    * **Draw:** Enter a route-drawing mode to click points on the map and create a custom route polyline.
    * **Reach:** Display the closest *saved custom route* to a specified destination.
* **Data Persistence:** All saved places and custom routes are persistent and specific to the logged-in user through Firebase Realtime Database.
* **Map Base Layer:** Uses Google Satellite imagery.
* **Multilingual Support:** Uses Hindi text for UI elements (e.g., login, register, place names).

---

## 🚀 Getting Started

### 1. Prerequisites

Before deploying or running this application, you must set up a **Firebase Project**.

* Create a new project in the [Firebase Console](https://console.firebase.google.com/).
* Enable **Email/Password** sign-in under **Authentication**.
* Initialize and set the security rules for the **Realtime Database**.

### 2. Configuration

Open the HTML file and update the `firebaseConfig` object within the `<script type="module">` tag with your own Firebase project credentials.

```javascript
// Firebase configuration (UPDATE THESE FIELDS)
const firebaseConfig = {
    apiKey: "YOUR_API_KEY",
    authDomain: "YOUR_AUTH_DOMAIN",
    databaseURL: "YOUR_DATABASE_URL",
    projectId: "YOUR_PROJECT_ID",
    storageBucket: "YOUR_STORAGE_BUCKET",
    messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
    appId: "YOUR_APP_ID",
    measurementId: "YOUR_MEASUREMENT_ID" 
};
●My algorithm my way, Ai just write Code.
