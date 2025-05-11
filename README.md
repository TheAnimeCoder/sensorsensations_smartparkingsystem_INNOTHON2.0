# IoT-Based Parking Management System

## Project Overview
The IoT-Based Parking Management System is a comprehensive solution designed to streamline vehicle entry, exit, and parking management processes. It leverages QR code technology, web applications, and IoT devices to provide a seamless parking experience.

## Features
- **Entry Gate System**: QR code scanning for vehicle entry.
- **Exit Gate System**: QR code scanning for vehicle exit.
- **Centralized Parking Management**: A web application for managing parking slots, user registrations, and payments.
- **User Authentication**: Secure login and registration system.
- **Real-Time Updates**: Live updates on parking slot availability.

## Folder Structure
```
ardiuno code/
  motor.ino
  position.ino

entry_gate/
  generateQRCode.js
  package.json
  README.md
  vehicleQRCode.png
  public/
    index.html
    css/
      style.css
    js/
      app.js
      auth.js
      scanner.js
  server/
    index.js
    seed.js
    controllers/
      authController.js
      parkingController.js
    middleware/
      auth.js
    models/
      ParkingEntry.js
      User.js
    routes/
      authRoutes.js
      parkingRoutes.js

exit_gate/
  generateQRCode.js
  package.json
  README.md
  vehicleQRCode.png
  public/
    index.html
    css/
      style.css
    js/
      app.js
      auth.js
      scanner.js
  server/
    index.js
    controllers/
      authController.js
      parkingController.js
    middleware/
      auth.js
    models/
      ParkingEntry.js
      User.js
    routes/
      authRoutes.js
      parkingRoutes.js

newparking/
  db.json
  eslint.config.js
  index.html
  package.json
  postcss.config.cjs
  README.md
  tailwind.config.js
  vite.config.js
  public/
    vite.svg
  src/
    AllRoutes.jsx
    App.css
    App.jsx
    Home.jsx
    index.css
    main.jsx
    assets/
      react.svg
      components/
        ContactSection.jsx
        FeaturesSection.jsx
        HeroSection.jsx
        HowItWorksSection.jsx
        Navigation.jsx
    components/
      ContactSection.jsx
      FeaturesSection.jsx
      Footer.jsx
      HeroSection.jsx
      Home.jsx
      HowItWorksSection.jsx
      Layout.jsx
      Login.jsx
      Navigation.jsx
      PrivateRoute.jsx
      Register.jsx
      SecondaryNavbar.jsx
      UserPage.jsx
      VehicleRegistration.jsx
      Wallet.jsx
    utils/
      fetchUserData.js
      generateQRCode.js
```

## Arduino Code

The `ardiuno code` folder contains the following files:

### motor.ino
This file controls the servo motors and IR sensors for the parking system. It includes:
- Servo motor initialization and attachment.
- IR sensor input handling.
- Serial communication setup.

### position.ino
This file manages the ultrasonic sensors and IR sensors for detecting vehicle positions. It includes:
- Pin definitions for multiple sensors.
- Path control logic.
- LED indicators for sensor status.

## Setup Instructions

### Prerequisites
- Node.js and npm installed on your system.
- A modern web browser.

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   ```
2. Navigate to the desired module (e.g., `entry_gate`, `exit_gate`, or `newparking`).
3. Install dependencies:
   ```bash
   npm install
   ```
4. Start the server:
   ```bash
   npm start
   ```
5. Open the application in your browser.

## Usage
- **Entry Gate**: Scan the QR code at the entry gate to register vehicle entry.
- **Exit Gate**: Scan the QR code at the exit gate to register vehicle exit.
- **Web Application**: Use the web interface to manage parking slots, user registrations, and payments.

## Technologies Used
- **Frontend**: HTML, CSS, JavaScript, React, Tailwind CSS
- **Backend**: Node.js, Express.js
- **Database**: JSON-based storage (for demonstration purposes)
- **Other Tools**: Vite, PostCSS, ESLint


---

Feel free to contribute to this project by submitting issues or pull requests.
