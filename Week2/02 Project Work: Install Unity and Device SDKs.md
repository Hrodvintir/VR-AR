# Project Work: Install Unity and Device SDKs

**For this project work, you will:**
 - Download and install the appropriate version of Unity

 - Download and install any SDKs you'll need to develop for your device

 - Configure your device for software development

### Instructions
Are you ready to take the first step toward creating an XR application? If you're an experienced Unity developer, you have probably completed these steps already and can skip this. If not, this project work will get you to the point where you can create a new project in Unity and run it on your mobile device.

If you run into any issues during this process, ask for help from your peers in the VR Project Build Help Forum.

### Step 1 - Install Unity
 - Visit the [Unity Download page](https://unity3d.com/get-unity/download) to begin the installation process. Select the "Choose your Unity + download" button. We do not currently recommend that you install the Unity Hub. 

 - Select the appropriate Unity license. For new developers, the free Personal Edition is most likely the correct choice.

 - Follow the instructions to download and run the Unity Download Assistant. We do not currently recommend that you install the Unity Hub.

 - During installation, on the "Unity component selection" page, select the components that are needed for your development platform. Enable "Android Build Support" if you will build to an Android device (Android-based smartphone, Gear VR, Oculus Go, Google Daydream, etc.). Enable "iOS Build Support" if you will build to an iOS device (iPhone). You should also enable "Vuforia Augmented Reality Support" to support the AR project work in this course.

 - Complete the installation and launch Unity

 - Create a new project to open the Editor. It doesn't matter what you call it, this will just be to complete the required configuration in the next step.

Reference these Unity resources for further information and troubleshooting tips for this step:

[Installing Unity without the Hub (Unity Manual)](https://docs.unity3d.com/Manual/InstallingUnity.html)

### Step 2 - Download and Install Device SDKs
Now you'll install the specific device Software Development Kit (SDK) that will enable Unity to work with your hardware device. 

**For Android development:**

If you will be creating your apps for an Android device (Android-based smartphone, Gear VR, Oculus Go, Google Daydream, etc.), follow these steps.

 - Visit the Android Developer site to [download Android Studio](https://developer.android.com/studio)

 - Follow the instructions to download, install, and open Android Studio

 - Note the location where the Android SDK is installed. You'll need to point Unity to this folder in a future step. You can find the location in the Android Studio SDK Manager. To open the SDK Manager from Android Studio, click Tools > Android > SDK Manager or click SDK Manager in the toolbar.

 - Back in Unity, using the top menu, navigate to Unity > Preferences (on OSX) or Edit > Preferences (on Windows).

 - When the Preferences window opens, navigate to External Tools.

 - Where it says Android SDK Location, click Browse, navigate to location of the directory containing the Android SDK Tools and click Choose.

Reference these Unity resources for further information and troubleshooting tips for this step:

 - [Building your Unity game to an Android device for testing](https://learn.unity.com/tutorials#5c7f8528edbc2a002053b4a2) (Unity tutorial)

 - [Getting started with Android development] (Unity Manual)

**For iOS development:**

If you will be creating your apps for an iOS device (iPhone), follow these steps. Note that a Mac is required to develop apps for iOS.

 - Visit the iOS developer portal to download [Xcode](https://developer.apple.com/xcode/)

 - Follow the instructions to download, install, and open Xcode, and to add your Apple ID to Xcode

Reference these Unity resources for further information and troubleshooting tips for this step:

 - Building your Unity game to an iOS device for testing (Unity tutorial)

 - [Getting started with iOS development (Unity Manual)](https://docs.unity3d.com/Manual/iphone-GettingStarted.html)

### Step 3 - Configure Your Device for Development (Android Only)
Finally, there are some additional steps to enable development mode on Android devices. This gives you access to various options related to building and debugging, and lets you test the game on your device.

The typical steps for Android smartphones are as follows:

 - On your Android device, navigate to Settings > About phone

 - Scroll to the bottom and then tap "Build number" seven times. A popup will appear, confirming that you are now a developer.

 - Now navigate to Settings > Developer options > Debugging and enable USB debugging.

This should prepare you to build a Google Cardboard app on your Android phone. Different steps are required for building apps for Oculus Go and Gear VR. Visit the Oculus Developer page for details:

  - [Oculus Go and Gear VR - Preparing for Mobile Development](https://developer.oculus.com/documentation/unity/unity-enable-device/)
