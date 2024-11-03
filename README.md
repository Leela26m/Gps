GPSLocator
Overview

GPSLocator is a real-time GPS tracking application built with Flutter. This app uses an ESP32 with a GPS sensor to send location data to ThingSpeak, which the app retrieves every 10 seconds to display the device's live location on a Google Map.
Features

    Real-Time Tracking: Updates location every 10 seconds, showing the ESP32’s current position.
    Google Maps Integration: Provides seamless map display and user-friendly navigation.
    ThingSpeak Connectivity: Utilizes ThingSpeak API for reliable data retrieval.
    User-Friendly UI: Intuitive interface for viewing and interacting with live location data.

Technology Stack

    Flutter: UI toolkit for building natively compiled applications across mobile, web, and desktop.
    Dart: The programming language used for Flutter development.
    ESP32 with GPS Module: Hardware for GPS data capture and transmission.
    ThingSpeak API: Cloud service for storing and accessing GPS data.
    Google Maps API: Map display and navigation.

System Architecture

    ESP32 with GPS Sensor: Captures and sends GPS data to ThingSpeak via Wi-Fi.
    ThingSpeak: Stores and provides access to the ESP32’s real-time location data.
    Flutter App: Fetches GPS data from ThingSpeak and displays it on a Google Map.

Screenshots

image
Getting Started
Prerequisites

    Hardware:
        ESP32 microcontroller with GPS module.
    Software:
        Flutter SDK (version 2.0 or above)
        Dart SDK
        Google Maps API key (from a Google Cloud project)
        ThingSpeak account and channel API key for data storage

Installation

    ESP32 Setup:
        Connect the GPS module to the ESP32.
        Program the ESP32 to read GPS coordinates and send data to ThingSpeak at intervals (e.g., every 10 seconds).

    ThingSpeak Configuration:
        Create a ThingSpeak channel and retrieve the Write and Read API keys.
        Confirm that the ESP32 is successfully sending data to ThingSpeak.
