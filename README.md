# 🛵 Food Delivery — Delivery Partner App

The Delivery Partner application is one of three mobile applications that make up the complete Food Delivery Platform.

It is designed for delivery partners to view available orders, accept deliveries, navigate to restaurants and customers, and complete deliveries using location and map-based functionality.

> 🍔 **Part of the complete Food Delivery Platform:**  
> [View the main project and complete platform architecture](https://github.com/hetpatel4902/food-delivery-platform)

## ✨ Features

### 🔐 Authentication

- Delivery partner registration
- Login
- Authentication using AWS Cognito
- AWS Amplify integration

### 📦 Order Management

- View available delivery orders
- Accept delivery requests
- View current delivery
- Manage active delivery workflow
- Complete delivery after reaching the destination

### 📍 Location & Navigation

- Detect current delivery partner location
- View delivery distance
- Navigate to the restaurant
- Navigate from the restaurant to the customer
- Display route information
- Share delivery location with the customer

### 🚚 Delivery Workflow

The application supports a two-stage delivery journey:

```text
Delivery Partner
       │
       ▼
View Available Orders
       │
       ▼
Accept Delivery
       │
       ▼
Navigate to Restaurant
       │
       ▼
Pick Up Order
       │
       ▼
Navigate to Customer
       │
       ▼
Reach Customer
       │
       ▼
Complete Delivery
```

## 🛠️ Technology Stack

- React Native
- JavaScript
- AWS Amplify
- Amazon Cognito
- Expo Location
- React Native Maps
- React Native Maps Directions
- React Navigation
- AsyncStorage
- NetInfo
- React Native Reanimated

The application is built using React Native 0.68.1 and includes AWS Amplify/Cognito, Expo Location, React Native Maps, and map-direction functionality. :contentReference[oaicite:2]{index=2}

## 📍 Location-Based Delivery

Location is a central part of the delivery workflow.

The application uses the delivery partner's current location to support:

- Distance calculation
- Restaurant navigation
- Customer navigation
- Route visualization
- Delivery location sharing

This allows the delivery process to be represented as a real-world journey from the delivery partner to the restaurant and then to the customer.

## 📁 Project Structure

```text
food-delivery-delivery-app/
│
├── component/
├── navigation/
├── screens/
├── src/
├── amplify/
├── android/
├── ios/
├── assets/
├── App.js
├── package.json
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Node.js
- React Native development environment
- Android Studio and/or Xcode
- Android/iOS device or emulator
- Required AWS configuration
- Required map service configuration

### Installation

```bash
git clone https://github.com/hetpatel4902/food-delivery-delivery-app.git
cd food-delivery-delivery-app
npm install
```

### Run the Application

Start Metro:

```bash
npx react-native start
```

Run on Android:

```bash
npx react-native run-android
```

Run on iOS:

```bash
npx react-native run-ios
```

> Note: The application depends on cloud services, location services, maps, and platform-specific configuration. Additional service configuration may be required.

## 🔗 Related Applications

This application is part of the complete Food Delivery Platform.

- 👤 [User / Main Platform](https://github.com/hetpatel4902/food-delivery-platform)
- 🏪 [Restaurant Partner App](https://github.com/hetpatel4902/food-delivery-restaurant-app)
- 🛵 **Delivery Partner App** — this repository
