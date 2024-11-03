# GPSLocator

## Overview
**GPSLocator** is a Flutter application designed to fetch and display real-time GPS data sent from an ESP32 with a GPS sensor. The ESP32 transmits location data to the ThingSpeak API, which the app retrieves every 10 seconds, allowing users to track their current position live on a Google Map.

## Features
- **Real-Time GPS Tracking**: Fetches and displays the ESP32 device's current GPS location every 10 seconds.
- **Google Maps Integration**: Utilizes the Google Maps API for a seamless mapping experience.
- **Live Updates**: Marks the current position on the map for easy navigation and tracking.
- **User-Friendly Interface**: Simple and intuitive UI for effortless interaction.

## Technology Stack
- **Flutter**: A UI toolkit for building natively compiled applications from a single codebase.
- **Dart**: The programming language used for Flutter development.
- **ESP32 with GPS Module**: Hardware for capturing and transmitting GPS data.
- **ThingSpeak API**: For storing and retrieving real-time GPS data.
- **Google Maps API**: For displaying the map and user location.

## Screenshot
![image](https://github.com/user-attachments/assets/d8fd871d-ced0-44df-8e31-0c4109fae0ad)

## Getting Started

### Prerequisites
- **Hardware**:
  - ESP32 microcontroller with GPS module.
- **Software**:
  - Flutter SDK (version 2.0 or above)
  - Dart SDK
  - A Google Cloud project with Google Maps API enabled
  - A ThingSpeak account with channel API keys

### Installation

1. **ESP32 Setup**:
   - Connect the GPS module to your ESP32.
   - Program the ESP32 to read GPS data and send it to ThingSpeak every 10 seconds.

2. **ThingSpeak Setup**:
   - Create a new ThingSpeak channel and note the Write and Read API keys.

3. **Flutter App Setup**:
   - Add your **Google Maps API key** in `AndroidManifest.xml`:
     ```xml
     <meta-data
         android:name="com.google.android.geo.API_KEY"
         android:value="YOUR_GOOGLE_MAPS_API_KEY"/>
     ```
   - Configure the app to use the **ThingSpeak Read API key** to fetch GPS data.

4. **Run the App**:
   ```bash
   flutter run
