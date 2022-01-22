# Project Work: There’s a Robot on Your Table

**In this project work, you will:**
 - Install the Vuforia SDK for building AR applications

 - Set up marker detection with an image target

 - Create a simple AR app that will show a 3D robot model through your smartphone camera when you point it at a special "target" that you'll print out. 

For this project, you will need an Android device running 4.4 or above, or an iOS device running 9 or above.

If you get stuck at any point in this project, you can seek help in the AR Project Build Help Forum.

## Instructions
### Step 1 - Install the Vuforia SDK
Let's get the Vuforia SDK working in a new Unity project. If you already downloaded the Vuforia SDK as part of Unity installation, you may be able to skip some or all of these steps.

 - In Unity, create a new 3D Unity project

 - Select Edit > Project Settings > Player

 - In the XR Settings roll-out menu, click on Vuforia Augmented Reality. This will download the correct version of the SDK for your Unity editor.

![alt text](https://github.com/Hrodvintir/VR-AR/blob/main/Week3/source/hMFcc3PwEei8FQ6TnIKJEA_8e78f6585382d2d7137972f7ce6b90f9_IMG_19062018_142221_0.png)

 - Install the SDK. You may be prompted to close the editor if it is open, or you may need to restart Unity for the changes to take effect.

***NOTE: In some versions of Unity, the Vuforia SDK installer mechanism seems to be broken. If that is the case for you, please re-install Unity, and select Vuforia support in the Unity installer modules. We apologize for any inconvenience.

 - Open your project in Unity and check the Vuforia Augmented Reality Box. A License Agreement dialog will appear.

![alt text](https://github.com/Hrodvintir/VR-AR/blob/main/Week3/source/oLEoHHPwEei8FQ6TnIKJEA_3a3161a3f5272f33dbced5b9299b3c82_IMG_19062018_142246_0.png)

### Step 2 - Add a Vuforia AR Camera to the Scene
 - In Unity, select GameObject > Vuforia > AR Camera. You will be prompted to install some additional assets, this will happen once per project. 

![alt text](https://github.com/Hrodvintir/VR-AR/blob/main/Week3/source/sNQEWHPwEeiMwApe4i-fLg_b30fba93d272cdbb47da4fa3fb2b1624_IMG_19062018_142302_0.png)

 - Delete the MainCamera object.

### Step 3 - Create an Image Target
Next, you'll add an image of the robot to a Vuforia database. This image will be the marker that the application is looking for to make the robot appear.

 - You will need to create a free Vuforia developer account on the Vuforia developer portal: https://developer.vuforia.com/vui/auth/register

 - Once registered, create a new developer key on their website by going to Develop > License Manager > Get Development Key. Name it “ARLesson”.

[Download](https://d3c33hcgiwev3.cloudfront.net/qlQAzXo0EeiLrA7SIbVCTg_aad58c507a3411e888a901059078d8a9_VuforiaAssets.zip?Expires=1642982400&Signature=Pt-RN4~u84XxBrL2o4VpnPUPidsr2HYTBiZ3YtkVMO4LAc7yb2k~k6oA2E60sIB6av4WPquy~JYjxHQ1C7ZD3gMJsMxNKkigyz0S4Df8HfPn65-BaeYbpCWfeJa6l2SUk6srPhDmcgsKovLdn~9KfEHKBLHuqA~N93jePUICeyQ_&Key-Pair-Id=APKAJLTNE6QMUY6HBC5A) the zip file below, which contains the assets you will need. After you unzip it, import it as a custom package to your Unity project.

 - Back on the Vuforia website, go to Develop > Target Manager > Add Database. Name it “VuforiaLesson_ImageTargets”.

 - Once the database is created, click on it and add a new target. Choose Single Image, browse for the ImageTargetRobot.jpg file, and set a width of 0.07 meters. Name it “Robot”.

 - Click on Download Database, then Download for Unity Editor. Import the resulting unitypackage file to your Unity project.

Here’s a tip! Vuforia benefits from having lots of trackable features which means zones of contrast in the target image. After the upload, each image will get a rating, like below.

![alt text](https://github.com/Hrodvintir/VR-AR/blob/main/Week3/source/NlbwnnPxEeiuCRJJ4_tQHA_64fe3090c15c2b3e5457f66d46e3b768_rating.jpg)

 - Go back to the Vuforia website and navigate to the License Manager page. Click on "ARLesson" and copy the license key. 

 - In Unity, find the VuforiaConfiguration asset in your project and paste the license key into the "App License Key" field.


![alt text](https://github.com/Hrodvintir/VR-AR/blob/main/Week3/source/Xys2VXPxEei8FQ6TnIKJEA_088d35b6117ba6bd5224a56a2628fef4_IMG_19062018_142321_0.png)

### Step 4 - Add the Targets to the Scene
Finally, you'll connect the image target to the Unity prefab that you want the app to show in augmented reality space, in this case a 3d robot model prefab.

1. In your Unity project, create an image target object by selecting: GameObject > Vuforia > Image

2. Configure the target to use the "VuforiaLesson_ImageTargets" database and then the "Robot" Image Target.
![alt text](https://github.com/Hrodvintir/VR-AR/blob/main/Week3/source/hj4cLXPxEeiuCRJJ4_tQHA_d4cbcc19969d3ffb56acbc779b38f947_IMG_19062018_142345_0.png)
3. Add the RobotAnimated prefab as a child of the image target. Make sure its local scale is 1.

4. Add the scene to the build in Build Settings and build to your device (make sure that your build target and other configurations match your device - revisit the project work in week 1 for more information). 

5. Print out a physical copy of the ImageTargetRobot.jpg. When you run your application, the 3D robot should appear when you point your smartphone camera at the image. Hello, Robot!
![alt text](https://github.com/Hrodvintir/VR-AR/blob/main/Week3/source/uNM3wnPyEeiMwApe4i-fLg_7d8df3375d334c98cd4a0db6dbab2877_Robot.png)
