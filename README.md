# TensorFlow Lite Object Detection Android - Aditya Ranjan
### Overview
This is a camera app that continuously detects the objects (bounding boxes and classes) in the frames seen by your device's back camera, using a MobileNet SSDV2 model trained on the custom dataset of Traffic lights, Traffic signs and Ambulance. These instructions walk you through building and running this repository on an Android device.

The model files are downloaded via Gradle scripts when you build and run. You don't need to do any steps to download TFLite models into the project explicitly.

Application can run either on device or emulator.

<!-- TODO(b/124116863): Add app screenshot. -->

## Build the app using Android Studio

### Prerequisites

* If you don't have already, install **[Android Studio](https://developer.android.com/studio/index.html)**, following the instructions on the website.

* You need an Android device and Android development environment with minimum API 21.
* Android Studio 3.2 or later.

### Building
* Open Android Studio, and from the Welcome screen, select Open an existing Android Studio project.

* From the Open File or Project window that appears, navigate to and select the tensorflow-lite/examples/object_detection/android directory. Click OK.

* If it asks you to do a Gradle Sync, click OK.

* You may also need to install various platforms and tools, if you get errors like "Failed to find target with hash string 'android-21'" and similar.
Click the Run button (the green arrow) or select Run > Run 'android' from the top menu. You may need to rebuild the project using Build > Rebuild Project.

* If it asks you to use Instant Run, click Proceed Without Instant Run.

* Also, you need to have an Android device plugged in with developer options enabled at this point. See **[here](https://developer.android.com/studio/run/device)** for more details on setting up developer devices.


### Model used
Custom trained model has been generated and placed in the assets folder. 

### Additional Note
_Please do not delete the assets folder content_. If you explicitly deleted the files, then please choose *Build*->*Rebuild* from menu to re-download the deleted model files into assets folder.

Big thank you to the TensorFlow Developer Community. 
Example android application code was used in this project with a custom tensorflow model generated for the purpose of the BE Final Year Project by Aditya Ranjan.
Feel free to use the code and model.
