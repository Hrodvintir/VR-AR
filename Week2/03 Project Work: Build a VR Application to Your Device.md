# Project Work: Build a VR Application to Your Device

### For this project work, you will:
 - Create a new Unity project and configure it to work with the course project package

 - Enable Virtual Reality support for your hardware configuration

 - Import the course project package, build it, and test it on your VR device

## Instructions
Make sure you complete the steps in the previous project reading to install Unity and set up your computer and mobile device for Unity development.

### Step 1 - Create a new Unity project
 - Open Unity and choose to create a new project

 - We suggest calling your project something like "vrMuseum" (but you can use whatever project name you want). Use the "3D" template to create your project so you don't include any unwanted packages or features.

### Step 2 - Install TextMesh PRO to properly render the text in the course project
We use TextMesh PRO in our project and you are highly encouraged to use it for your own projects as well. It is now a free Unity asset and you may need to enable it using the new Package Manager in Unity.

 - If you are using 2018.2 or later, TextMesh PRO may be pre-installed and you will not need to install it. Otherwise continue with the steps below.

 - In the Unity Editor file menu, select Window > Package Manager and select the "All" tab on the left hand panel. This shows available packages for import. Select TextMesh PRO from the list and install it.

### Step 3 - Enable Virtual Reality Support in Unity
We need to enable XR features in Unity before our project will run on VR headsets. 

 - In Unity, open the Player Settings panel by selecting Edit > Project Settings > Player from the file menu. The Player Settings window will open in the Inspector. In the default Unity layout, this is on the right side of the page.

 - To build to an Android device, click the Android icon in this window to open the Settings for Android menu. To build to an iOS device, click the icon that looks like an smartphone to open the Settings for iOS menu.

 - Regardless of which menu you picked, Virtual Reality support is enabled by clicking the XR Settings roll-out menu, and checking the "Virtual Reality Supported" box. Checking this box will activate a list of Virtual Reality SDKs. The list will be empty at first.

 - Click the plus sign at the bottom right of the empty list and select "Cardboard." This will enable support for Google Cardboard devices.

 - Make sure that the "Stereo Rendering Method" is set to "Single Pass" (iOS) or "Single Pass Multiview or Instanced" (Android)

 - In addition, for Android devices, open the Other Settings roll-out menu and make sure that Color Space is set to "Gamma" (linear color space is not supported by many mobile devices), and update the Company and Product Name in the Package Name field to something logical (for example "com.YourName.vrMuseum"). Finally, set the Minimum API Level to "Android 4.4 'Kit Kat' (API Level 19).

### Step 4 - Import the VR Museum Unity Package
Next you'll download and import the Unity project files for this application.

 - Download the file below and unzip it:
 *[vrMuseumPackage](https://d3c33hcgiwev3.cloudfront.net/KOuBb5QFEei-ewqCW6OQ9g_2968ee10940511e88bda2587e80496e2_vrMuseumPackage.zip?Expires=1642982400&Signature=PaUNsHuWbPDK4ou4JG0OoP6Q1Wy3gIUWRLRN8y8lCTlX3iUnMIZ6-ZnZ0exOlmw86UZ1W7cXUg3V26OrW9uY35SKVZBFE9KmHsSy-YySyn72CnPiTVpXkav4uh5xohJD9uoRJwzYJpHBjhS5JoWkQoKG~S~OU5-1JWBR~aswppU_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A)*
 
 - In Unity, select Assets > Import Package > Custom Package

 - Locate and open the vrMuseum.unitypackage that you just extracted.

 - When the Import Unity Package window appears with a list of all of the assets in the package, just click the Import button on the bottom right. This will import all assets in the package.

### Step 5 - Open and explore the VR Museum scene
 - In the Project Window (bottom left for the default Unity layout), find the vrMuseum scene within the Assets > vrMuseum > scenes folder. Double click the vrMuseum scene file (not the folder of the same name) to open it.

 - You may be prompted at this point to import some additional TextMesh Pro resources. Click the button to "Import TMP Essentials". Then close the TMP Importer window by clicking the red bubble button in the top left corner of that window.

 - The scene should open in the Scene window. If you're familiar with Unity's user interface, feel free to take a look around the scene. If you're less familiar, this Unity tutorial on Interface Essentials will help you get your bearings.

### Step 6 - Build and run the VR Museum application on your device
 - In Unity, select File > Build Settings

 - In the Build Settings menu, you'll first identify the scenes to include in the build. Uncheck the box next to "Scenes/SampleScene" if it is included and click the "Add Open Scenes" button to add the vrMuseum Scene. 

 - Next, select the appropriate platform - Android or iOS - in the Platforms list, and click the "Switch Platform" button.

 - Moment of truth! Connect your smartphone to your computer via USB and click "Build and Run." Wait a little while as Unity builds and deploys the app to your device (or a long while - this process should be faster on subsequent builds). Once it's done, the app should launch on your phone. Put it in a Cardboard viewer to experience it. We'll take you on a guided tour in a later lesson.
