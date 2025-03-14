# CSCI712
Introduction 

I'm excited to share my latest Android project, which demonstrates the requirements for Assignments 2 and 4 of my mobile software engineering course. This project uses Kotlin, Jetpack Compose, and Android Studio.

Table of Contents

Assignment 2 Overview Assignment 4 Overview Project Structure How to Run Screenshot for Assignment 4 Assignment 2 Overview

For this assignment, I had to create an app with two activities: MainActivity and SecondActivity. MainActivity displays my full name and student ID, along with two buttons: "Start Activity Explicitly" and "Start Activity Implicitly". The first button directly starts SecondActivity, while the second button starts it via an implicit intent action. SecondActivity lists five mobile software engineering challenges and has a button that navigates back to MainActivity.

I successfully created and ran the app, and I'm happy to report that it works as expected. The implementation highlights include:

MainActivity, which uses Jetpack Compose to display my name and ID, along with the two buttons. SecondActivity, which also uses Jetpack Compose to display the five challenges and the "Main Activity" button. The AndroidManifest.xml file, which declares both activities and includes an intent-filter for the implicit action. Assignment 4 Overview

For this assignment, I added a new button to MainActivity called "View Image Activity", which opens ThirdActivity. ThirdActivity has a "Capture Image" button that opens the camera, and after taking a photo, it displays the captured image. I had to run the app on a device or emulator, take a screenshot of the third activity displaying the captured image, and commit the code to the existing GitHub repository.

The implementation highlights include:

ThirdActivity, which uses an implicit intent to open the camera. The image capture functionality, which returns a thumbnail of the captured image and displays it in an Image composable below the capture button. The placeholder text or black bitmap that is shown if no image has been captured yet. Project Structure

The project is structured as follows:

app/src/main/java/com/example/assignment2 contains the Kotlin files for the three activities: MainActivity, SecondActivity, and ThirdActivity. app/src/main/res contains the resources for the app, including layouts, drawables, and values. AndroidManifest.xml declares all three activities and intent-filters. build.gradle contains the build configuration for the app. How to Run

To run the app, follow these steps:

Clone the repository using the command git clone https://github.com/xnoodlexboyx/712App.git. Open the project in Android Studio. Build and run the app using either an Android emulator or a physical device with USB debugging enabled. On the main screen, you can start Activity Explicitly or Implicitly, or open ThirdActivity using the "View Image Activity" button. In ThirdActivity, you can tap the "Capture Image" button to open the camera and take a photo. The captured image will be displayed on the screen.
