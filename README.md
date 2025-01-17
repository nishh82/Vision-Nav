# VisionNav: AR-Based Indoor Navigation Application

![VisionNav Logo](https://i.ibb.co/QNCy761/Screenshot-2024-08-04-at-6-08-17-PM.png)

## Overview

VisionNav is an innovative Augmented Reality (AR) based indoor navigation application designed to tackle the challenges of navigating large, complex indoor environments. Developed by a team of researchers at the University of Windsor, this project integrates cutting-edge AR technology with robust database management and pathfinding algorithms to provide an intuitive and immersive wayfinding experience.

## Features

- **AR-Enhanced Navigation**: Overlays digital directional cues onto the user's real-world view.
- **QR Code Localization**: Utilizes strategically placed QR codes for accurate positioning.
- **SLAM Integration**: Implements Simultaneous Localization and Mapping for real-time environment mapping.
- **NavMesh Pathfinding**: Employs Unity's NavMesh tool for efficient route calculation.
- **Dynamic Obstacle Avoidance**: Real-time path adjustments for unexpected obstacles.
- **Multi-Floor Navigation**: Seamless guidance across multiple levels of a building.
- **User-Friendly Interface**: Intuitive design suitable for users of all technical proficiencies.

## Technology Stack

- **Frontend**: Unity, ARCore
- **Backend**: Node.js
- **Database**: MongoDB
- **AR Framework**: ARCore
- **3D Modeling**: Blender
- **Version Control**: Git

## Installation
1. Clone the repository:
2. Install Unity 2020.3 LTS or later.
3. Open the project in Unity.
4. Install the following Unity packages:
- ARCore
- ARFoundation
- NavMeshComponents
5. Set up the backend:
- Install Node.js and npm
- Navigate to the backend directory
- Run `npm install` to install dependencies
6. Set up the database:
- Install MongoDB
- Create a new database named "visionnav"
- Import the provided map data and QR code locations
7. Configure the connection strings in the Unity project to point to your backend server and database.

8. Build the project for Android (minimum API level 24).

## Usage
1. Install the VisionNav app on your Android device.

2. Launch the app and grant necessary permissions (camera, location).

3. Navigate to an entrance point of the building where a QR code is located.

4. Scan the QR code to initialize your location:
- Hold your device steady and point the camera at the QR code
- The app will vibrate and display a confirmation when successfully scanned

5. Once your location is initialized, use the search function to select your destination.

6. Follow the AR overlay instructions:
- Directional arrows will guide you along the optimal path
- Waypoints will indicate key turning points or landmarks

7. If you encounter an obstacle, the app will automatically recalculate your route.

8. For multi-floor navigation:
- Follow the AR indicators to the nearest staircase or elevator
- The app will guide you to the correct floor and continue navigation

9. If you deviate from the suggested path, the app will recalculate and provide updated directions.

10. Upon reaching your destination, the app will display a confirmation message.

Note: Ensure good lighting conditions for optimal QR code scanning and AR performance. If you experience any issues with localization, try rescanning the nearest QR code.

## Demo

![Demo GIF](path_to_demo_gif.gif)

Check out our [video demo](https://ik.imagekit.io/abhishekrma7/VisionNav-Demo?updatedAt=1722809666978) for a comprehensive look at VisionNav in action.

## Performance Metrics

- **Localization Accuracy**: ±1.2 meters
- **Average QR Code Scan Time**: 1.5 seconds
- **Pathfinding Calculation Time**: 0.3 seconds
- **Frame Rate**: 30-60 FPS (device-dependent)
- **AR Positioning Drift**: <0.5 meters per 100 meters traveled

## Challenges and Future Work

- Improving performance in dynamic environments
- Enhancing QR code scanning in various lighting conditions
- Expanding entry point options for navigation initialization
- Implementing voice assistant features for improved accessibility
- Extending support to iOS devices

## Team

- Abhishek Solanki (Team Lead) - [GitHub](https://github.com/abhishek-rma7)
- Meet Patel
- Harshkumar Sabhaya
- Nishant Jethva

## Acknowledgements

We would like to thank the University of Windsor for their support and resources in making this project possible.

## License

This project is licensed under the [MIT License](LICENSE).
