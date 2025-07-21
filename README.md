## Resources

**Read or watch**:

*   [Dart - Cheatsheet](/rltoken/vNcJwx9uH1oO97J3weOg2Q "Dart - Cheatsheet")
*   [FlutterFire Overview](/rltoken/2pqfv23C5fIPlhQuc8-lzw "FlutterFire Overview")
*   [Getting started with Firebase on Flutter](/rltoken/HT04HWjRJGP6J-TRB6USKA "Getting started with Firebase on Flutter")
*   [Get Started with Firebase Authentication on Flutter](/rltoken/RPOfxJurI2FTxqvM3_Rz7g "Get Started with Firebase Authentication on Flutter")
*   [Cloud Storage on Flutter](/rltoken/P6NOA7DAhr4Nj51tnZxaFQ "Cloud Storage on Flutter")
*   [Layouts in Flutter](/rltoken/w2ZjcQ9A0uJy4l1z2sehcQ "Layouts in Flutter")
*   [Introduction to widgets](/rltoken/bnUF2_6TmceGXZgRMpyW_A "Introduction to widgets")
*   [Cloudinary Storage Images uploading | Flutter](/rltoken/MemgVBz8hW7Rh5Ty_qtpbA "Cloudinary Storage Images uploading | Flutter")

**Every Flutter Widgets**

*   [Every Flutter Widget Explained](/rltoken/pUuGD0ZBuuTUsLAsubY2hA "Every Flutter Widget Explained")

## Requirements

**Create your project :**

Open you’re command-line tool

*   `flutter create holbegram`
*   `cd holbegram`
*   `flutter run`

**Step up your Firebase**

For the backend, we are going to use Firebase(Firebase is a Backend-as-a-Service (BaaS) app development platform that provides hosted backend services such as (`a real-time database`, `cloud storage`, `authentication`, `crash reporting`, `machine learning`, `remote configuration`) and hosting for your static files. However, for storing and managing images, we will use Cloudinary, which is a cloud service that provides an easy-to-use solution for managing images and videos, including features for storing, transforming, and delivering media content. Cloudinary will handle the storage and retrieval of image files, while Firebase will handle the authentication and database functionalities.

Let’s start…

go to `https://firebase.google.com/` and create an account then Let’s create a new project in firebase.

Go to Firebase Console and click Add Project and then you have to go through some steps.

**First**, we are going to build a fire\_base app called `holbegram`:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/effcaadc5053cd0f13321f3da0ca7af485e48499.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=02525f8d4937693f867d6ce57b7e19e28ae41e21571f7db882c252acaaf2071c)

**Second** Disable Google Analytics for this project:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/75475181f194def86264d0898b5ccde396c21725.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ff7d2cf05d9537b0b0837f5fd418709e72fa9835b25a66d86f3b23173bd84b91)

**Authentication**

Click on Enable the Authentication: Enable the Email/Password

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/b25d3fd7c4d0bd2ffb3dd8308ecaf22f00794548.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=5cf5b59750800f3c7c39f3ee5ccd882040bd71c39f0fd64e61b87b80ea06edec)

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/7f78a5264c27e64db051eeec0edd2ed872c9beba.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=13fa9cdb73229722fa95623966a8ca73f7446ec49493ebaffafb6dcd4e14c6bb)

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/60f7d7c2e8b28345beb62365d71a737182693ff2.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=54ca6aae2b33797111b2869bcdbcecd7c668e6b3aa1e89825314614803951e22)

**Database**

Well done! Now you are going to move to the next task which is creating a database.

To do that follow the following steps:

1- Go to Firestore Database then click on Create Database.

2- Choose “start in test mode”

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/fcb8a7236705b8a58455fa12972d20c66712cf64.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=071bfb29c26018fb2b81d587ce59a1cda7d1a3da5fce041983eb763d9b6edca1)

3- choose the location that is close to you.

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/2cccf7ed30807a79d66640d0c862b62b41e28750.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ec2e1d2465c96de3a10a18bde612c6e3fa29bd472ac700910980c9e027049269)

4- Go to rules:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/ee6587e9101eb092270dbe1582bfc85bfc951c95.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=369828a6659643ba45fdb8a77af0654268f11f3e3b3a03587f2ea43054326623)

Finally, press Publish

**Adding Firebase to our AppSo now let’s add Firebase to our app:If you want to use Android Follow the Android SupportIf you want to work with iOS follow the iOS Support**

# **Adding Android support**

Registering the App

In order to add Android support to our Flutter application, select the Android logo from the dashboard. This brings us to the following screen:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/79c7e4222312d48e0c162322f2d138f476e2d0c0.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f66cb3337910a193d2f6240a9fb5f1b7fba8f2fd39581fd2a6c5c81cff422e5b)

The most important thing here is to match up the Android package name that you choose here with the one inside of our application.

The structure consists of at least two segments. A common pattern is to use a domain name, a company name, and the application name:

`com.example.holbegram`

Once you’ve decided on a name, open `android/app/build.gradle` in your code editor and update the applicationId to match the `Android package name`:

Example of File `android/app/build.gradle`
```
...
defaultConfig {
    // TODO: Specify your own unique Application ID (https://developer.android.com/studio/build/application-id.html).
    applicationId 'com.example.holbegram'
    ...
}
...
```
You can skip the app nickname and debug signing keys at this stage. Select Register app to continue.

**Downloading the Config File**

The next step is to add the `Firebase configuration` file into our Flutter project. This is important as it contains the API keys and other critical information for Firebase to use.

Select Download `google-services.json` from this page:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/29220467a87b78d62f287d431dc5c308470c01b9.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=4e725e3b68ca4466041c36b72e3c0e973083541c28e2d74b7e0d094b37fe865a)

Next, move the `google-services.json` file to the `android/app` directory within the Flutter project.

**Adding the Firebase SDK**

We’ll now need to update our Gradle configuration to include the Google Services plugin.

Open `android/build.gradle` in your code editor and modify it to include the following:

Example of File `android/build.gradle`
```
buildscript {
  repositories {
    // Check that you have the following line (if not, add it):
    google()  // Google's Maven repository
  }
  dependencies {
    ...
    // Add this line
    classpath 'com.google.gms:google-services:4.3.13'
  }
}

allprojects {
  ...
  repositories {
    // Check that you have the following line (if not, add it):
    google()  // Google's Maven repository
    ...
  }
}
```
Finally, update the app level file at`android/app/build.gradle` to include the following:

Example of File `android/app/build.gradle`
```
apply plugin: 'com.android.application'
// Add this line
apply plugin: 'com.google.gms.google-services'

dependencies {
  // Import the Firebase BoM
 implementation platform('com.google.firebase:firebase-bom:30.2.0')

  // Add the dependencies for any other desired Firebase products
  // https://firebase.google.com/docs/android/setup#available-libraries
}
```
With this update, we’re essentially applying the Google Services plugin as well as looking at how other Flutter Firebase plugins can be activated such as Analytics.

From here, run your application on an Android device or simulator. If everything has worked correctly, you should get the following message in the dashboard:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/eca3dbd42b0d5c6af14cb2292bb7ef321b9d6fa3.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=36064f4dc86a3cf0f833e9d5a8f610f0085a2dde84c1abe03d8a31861ff7cdb5)

# **Adding iOS support**

In order to add Firebase support for iOS, we have to follow a similar set of instructions.

Head back over to the dashboard and select Add app and then iOS icon to be navigated to the setup process.

**Registering an App**

You Should have **Xcode** installed in your PC:

Once again, we’ll need to add an “iOS Bundle ID”. It is possible to use the “Android package name” for consistency:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/f45889853f3e6c71ef12e7a13889c9378e89c472.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=4237556cfec9c5708a364535de69c30b87201381288d5a89193af5b2149ab797)

You’ll then need to make sure this matches up by opening the iOS folder up in `Xcode`

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/9d7946cee42b4fe2f94cd07c95c42b3a58f1285f.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=d11872db274ff74fe6d80e5c9f5d6e2249e86d62953ebd5349a87b0823e8a69b)

*   General

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/83c1b8343fb170c1162d3eb0d022aa50fb04ce06.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=773a300bf145b579b940fd9abc511dd14443c2d9a913451fcdc43cce484915fa)

Now go back to your firebase and add the iOS Bundle ID

after that Download the configuration file

**Downloading the Config File**

Drag and Drop the file `GoogleService-Info.plist` and move this into the root of your Xcode project within `Runner`:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/b13f1b0452f1145f980d439a4dcda17a2d4d0f5c.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=5bba1ead8db7b863ae6d93ab0c3bf7ca84f9e1123806dfa9bab90b5a72896dbd)

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/d8d7fb980a6bf8db79fca2b2f029d4f423767b80.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=29358e1ae997dfb2ca36db38b05a727b0d86ed1ceaef2cfa2277f9d6a4d005ca)

Be sure to move this file within Xcode to create the proper file references.

## Tasks

### 1.

Now after we set our Firebase we gonna start build our Application, First we are going to create Three screens `Login Page` `Sign up Page` and `Upload image Page`.

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/138de426ea182abb86ae90b76e6517ab4794ba2a.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=fe7486e69de392bccbef3a7c3f2fd6a6071a0190d551655d42d1221b70a3d24b) ![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/c8e3e89811dfc10d61c27bf5be23cfbf1eb8ca99.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=4a97a969d8a4007818418a43190489fee17823b95d61cc986cba25fe70112d00) ![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/b15f8b2a55c6d8ba52fe0adf343bc5acd40a2ceb.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e2818c80f4c6bd310b26de09e80b8b2c41393719695dd108cc0b5aa09065c78e)

**In your lib folder**:

*   create new folder named **screens**:
    *   inside the **screens** folder create 3 files named:
        *   login\_screen.dart
        *   signup\_screen.dart
        *   upload\_image\_screen.dart

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/09362f244f473704661a68ffa94e15bcd3ecd97d.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=3dadadd9e815e7d4e3d2e9606a830af7919b90e1df2b426d8a42f91d03af807b)

*   create new folder named **widgets**:
    *   inside the **widgets** folder create 1 file named:
        *   text\_field.dart

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/c3a2e750023c4588d8e57fe57fb327183a9df5bb.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=5a50686000cd9935dc2271a9f7b067acefc0cc40e3cf91dad4ecdbdf8a5351ba)

**Initialization App**

Install these packages:

*   [firebase\_auth](/rltoken/PCtSeP6u5iTMeYF2GCkuQg "firebase_auth") : `flutter pub add firebase_auth`
*   [firebase\_database](/rltoken/XxBGYPjJR_VnypLH1WKkDw "firebase_database") : `flutter pub add firebase_database`
*   [cloudinary\_flutter](/rltoken/Kkv6W9cD9E26zqpnJxR7gg "cloudinary_flutter"): `flutter pub add cloudinary_flutter`

Change the function`void main()` to:
```
Future main() async {
  WidgetsFlutterBinding.ensureInitialized();
  await Firebase.initializeApp();
  runApp(const MyApp());
}
```
  

### 2.

In the `widgets/text_field.dart` :

In order to learn how a reusable widget works, we will build this TextField widget .

Create a new `StatelessWidget` called `TextFieldInput` with these attributes:

*   `controller`: TextEditingController
*   `ispassword`: bool
*   `hintText`: String
*   `suffixIcon`: Widget it cloud be `null`
*   `keyboardType`: TextInputType

After the `Widget build`

Return `TextField()`:

*   `keyboardType` takes `keyboardType`
*   `controller` takes `controller`
*   `cursorColor` takes `Color.fromARGB(218, 226, 37, 24)`
*   `decoration` takes `InputDecoration`:
    *   `hintText` takes `hintText`
    *   `border` takes `OutlineInputBorder`:
        *   `borderSide`: `BorderSide`
            *   color : transparent
            *   style: none
    *   `focusedBorder`: `OutlineInputBorder`
        *   `border` takes `OutlineInputBorder`:
            *   `borderSide`: `BorderSide`
                *   `color` : `transparent`
                *   `style`: `none`
    *   `enabledBorder`: `OutlineInputBorder`
        *   `border` takes `OutlineInputBorder`:
            *   `borderSide`: `BorderSide`
                *   `color` : `transparent`
                *   `style`: `none`
    *   `filled` : `true`
    *   `contentPadding` : `EdgeInsets.all(8)`
    *   `suffixIcon` takes `suffixIcon`
*   `textInputAction` : `next`
*   `obscureText` takes `ispassword`

For Example :

If we put the `hintText` : `Email` it’s giong to be like this:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2023/1/9b678015040ae3573a5cec7de257eae6d9992254.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=524a5229837e5a22e438f5962aa1144432732e09322640744519148d4f1f267a)

Another Example :

If we put the `hintText` : `Password` and `ispassword`: `true` it’s giong to be like this:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2023/1/48113af9741c78b783e988135934a252c8da6c61.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=deda71c5a8ddf0b8f47bdf6bf1b3445be78d006567e9297383eadf48f5622dae)

  

### 3.

Login Page

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2023/1/e80a4da25022391cd487de3ca468c0ea499bd2b0.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6d850a276031d89d62355df8b756804d5e887bb9bd194f5caf3b38e96a1c2be2)

You will need this [Logo](/rltoken/7_1UNJISW2XoioyxNbfB_w " Logo") and this [Font](/rltoken/tuT3KosLdbfQHRl_vZk0OQ "Font")

After That Create two folders inside the `assets` :

*   `images`
*   `fonts`

Put the Logo inside the Images folder and Billabong fonts inside the fonts folder

Inside the `pubspec.yaml`

*   add this `- assets/images/` under the `assets`:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/75ae4cad40cc06dc44676aa49cbd43ebf32e654c.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=0fc2c25b9459a874029fa46fa1ca884bdd9ddacd50830efaca911062f73db028)

*   add this under the fonts
```
- family: Billabong
      fonts:
        - asset: assets/fonts/Billabong.ttf
        - asset: assets/fonts/InstagramSans.ttf
```
![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/11/be4ca97fb69abb3065edd3587478bef1d7e8ad43.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=1877dbbcbea795c8f630329debb87c09ed6645b249dc64b7f88d13a4ba60b700)

**Now** Inside `login_screen.dart` :

*   Create a new `StatefulWidget` called `LoginScreen` that takes these arguments.
    *   `emailController` : `TextEditingController`
    *   `passwordController`: `TextEditingController`
    *   `_passwordVisible` : `bool` default takes `true`

**Dispose** only the `TextEditingController` arguments

**initState** for the `_passwordVisible`, before that, you add `@override` annotation

*   Returns: `Scaffold()` Inside the scaffold add a `SingleChildScrollView` in the body
    
    *   `SingleChildScrollView` takes `Column`:
        *   `Horizontally of the Column will be : min`
        *   `Verticale of the Column will be : center`
    *   Inside of the `Column` :
        
        *   `children[]`:
            
            *   Set the `SizedBox` of `height` to `28`
            *   Create a Text widget that contains the name of the app `Holbegram` with the `Billabong` Font and the font size of `50`
            *   The logo will be inside an Image widget (`width: 80,height: 60`)
            *   Create `Padding`
                *   Set `EdgeInsets.symmetric` to `horizontal` : `20`
                *   Child takes a `Column`
                *   Inside the `Children` of the `Column` we are going to call the `TextFieldInput` that we created. First let’s keep our screen Sized
            *   `SizedBox` takes height: `28`
        *   Email `TextFieldInput`
            
            * `controller` : `emailController`
            
            * `ispassword` : flase
            
            * `hintText` : `Email`
            
            * `keyboardType` : `TextInputType.emailAddress`
            
    *   Set the `SizedBox` of `height` to `24`
        
    *   Password `TextField`
        
        *   `TextFieldInput`
            *   `controller` : `passwordController`
            *   `ispassword` : `!_passwordVisible`
            *   `hintText` : `Password`
            *   `keyboardType` : `TextInputType.visiblePassword`
            *   `suffixIcon` takes `IconButton`
                *   `alignment` : `bottomLeft`
                *   If the `_passwordVisible` is `ture` `icon` takes `visibility` or `icon` takes `visibility_off`
                *   use setState inside the `onPressed: ()` to change the `_passwordVisible` when pressed
*   Set the `SizedBox` of `height` to `28`
    
*   `SizedBox`
    
    *   `height`: `48`
    *   `width` : `double.infinity`
    *   `child` : `ElevatedButton`:
        
        *   `style`:
            *   `ButtonStyle`
                *   `backgroundColor` :`WidgetStateProperty.all(Color.fromARGB(218, 226, 37, 24),)`
        *   `onPressed` leave it empty for the moment
        *   `child` : `Text`:
            *   `Log in`
            *   `style`:
                *   `TextStyle(color: Colors.white)` After this.
*   Set the `SizedBox` of `height` to `24`
    
*   `Row`
    
    *   `mainAxisAlignment`: `center`
    *   `children`:
        *   `Text` : `Forgot your login details?`
        *   `Text` : `Get help logging in` with `fontWeight` : `bold`
*   `Flexible`:
    
    *   `flex`: `0`
    *   `child`: `Container()`
*   Set the `SizedBox` of `height` to `24`
    
*   `Divider` : `thickness` to `2`
    
*   `Padding`:
    
*   Set `vertical` padding to `12`
    
*   `child` takes `Row`:
    
    *   `mainAxisAlignment`: `center`
    *   `children`:
        *   `Text` : `Don't have an account`
        *   `TextButton`:
            *   `onPressed` leave it empty for the moment
            *   `child` takes `Text` with a String `Sign up` set `fontWeight` to `bold` and `color` to `fromARGB(218, 226, 37, 24)`
    *   Set the `SizedBox` of `height` to `10`
*   `Row`:
    
    *   `children`:
        *   Create two `Flexible` widgets with `child` takes `Divider` : `thickness` to `2` between the two widget create a `Text` with string `" OR "`
*   Set the `SizedBox` of `height` to `10`
    
*   `Row`:
    
    *   `mainAxisSize` : `min`
    *   `mainAxisAlignment` : `center`
    *   `children`:
        *   Takes an Image network with `width: 40` `height: 40`
            *   Image : [Image Link](https://www.freepnglogos.com/uploads/google-logo-png/google-logo-png-webinar-optimizing-for-success-google-business-webinar-13.png "Image Link")
        *   `Text` : `"Sign in with Google"`

  

### 4.

Signup Page

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2023/1/24850d82e5025b87cfe2401b37504c7f9f729ab7.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=7ceeccda0ca9ccbc191a6653dbe48c77f35c3b2c6f56900418913e2f2fb130b5)

Inside `signup_screen.dart` create :

*   Create a new `StatefulWidget` called `SignUp` takes these arguments.
    *   `emailController` : `TextEditingController`
    *   `usernameController` : `TextEditingController`
    *   `passwordController`: `TextEditingController`
    *   `passwordConfirmController`: `TextEditingController`
    *   `_passwordVisible` : `bool` default takes `true`

Let’s `dispose` them like we did in the Login Page and don’t forget `initState` for the `_passwordVisible`

Now! we are going to do the `Sign Up` page. It is very similar to the previous task therefore, I want you to try this on your own.

If you face any difficulties check the previous task or do as any great developer does: Google it!

In the bottom there is a String “Log in”

It’s a `TextButton` that navigates you to the Log in page

If you want to do it alone it’s a plus too or jump to the next task.

  

### 5.

Inside `login_screen.dart`:

In the `TextButton` widget that contains`Sign Up` as a `Text`

we will change the `onPressed` to make it navigate to the Sign Up page:

*   Use `Navigator.push`:
    *   Assign `SignUp()` and don’t forget to import it

Inside `signup_screen.dart`

In the `TextButton` widget that contain`Log in` as a `Text`

we will change the `onPressed` to make it navigate to the Log in page:

*   Use `Navigator.push`:
    *   Assign `LoginScreen()` and don’t forget to import it

  

### 6.

In the `lib` folder:

*   Create a new folder called `models` that contains two file :
    *   `user.dart`
    *   `posts.dart`

In the `lib/models/user.dart` create a class called `Users`:

*   Properties:
    *   `uid`: String
    *   `email`: String
    *   `username`: String
    *   `bio`: String
    *   `photoUrl`: String
    *   `followers`: List`<dynamic>`
    *   `following`: List`<dynamic>`
    *   `posts`: List`<dynamic>`
    *   `saved`: List`<dynamic>`
    *   `searchKey` : String

Create a new instance called `fromJson` that accepts `DocumentSnapshot` as parameter

*   Prototype :
    *   `static Userd fromSnap(DocumentSnapshot snap)`

Create a variable inside the `fromJson` called `snapshot` that is going to take the data from `snap`

Return every value inside it.

Create a method called `toJson()` that returns a map representation of the `Users`

  

### 7.

Create a new folder inside the `lib` called `methods`:

Inside `lib/methods` create a new file called `auth_methods.dart`

Now inside `auth_methods.dart`:

Start by adding the packages needed :

*   `Cloud_firestore`
*   `Firebase_auth`
*   `http (for Cloudinary API requests)`
    
*   Create a new Class called `AuthMethode` that’s going to contain our Methods.
    

Inside the class, create two arguments:

*   `_auth` that extends from `FirebaseAuth`
*   `_firestore` that extends from `FirebaseFirestore`

`_auth` = `FirebaseAuth.instance`

`_firestore` = `FirebaseFirestore.instance`

Create a new instance for Login called `login` that takes two arguments `email`: String, `password`: String. Return a String

*   Prototype :
    *   `Future<String> login({required String email,required String password,})`
        *   Check if the email or the password are empty:
            *   Return `Please fill all the fields`
        *   Use `_auth.signInWithEmailAndPassword` method from `FirebaseAuth`
        *   Return `success`
            *   On success navigate to the home screen

Now go back to the login screen and edit the submit button to call login() while passing the corresponding parameters and use the function’s return value to show a snackbar with the text “Login” on success

Create a new instance for Sign Up called `signUpUser` that takes these arguments `email`: String , `password`: String , `username`: String , `file`: Uint8List. Return a String

*   Prototype :
    *   `Future<String> signUpUser({required String email,required String password,required String username,Uint8List? file,})`
        *   Check if the `email` or the `password`, `username` are empty:
            *   Return `Please fill all the fields`
        *   Use `_auth.createUserWithEmailAndPassword` method from `FirebaseAuth`
        *   `userCredential` takes the return of the `_auth.createUserWithEmailAndPassword`

**Now** right! after using `_auth.createUserWithEmailAndPassword` put this:

*   `User`takes `userCredential.user`;

The arguments that we just passed in to Sign Up put it to our `Users` Class

After that:

*   `await _firestore.collection("users").doc(user.uid).set(users.toJson());`
*   Return `success`

  

### 8.

Let’s put our file in the `screens` inside a new folder called `auth` :

Create a new folder inside `screens/auth` called `methods`:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2023/1/197d8d071c1bf504f62185889aaeb1e7268a43c7.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=7a5790993734e673c7d03c111f4e1c245d1a542b1ea1f00be2762fbedecc2d1a)

Inside `methods` folder create a new file called `user_storage.dart`:

Copy and paste the Code into your file
```
import 'dart:typed\_data';
import 'package:uuid/uuid.dart';
import 'package:http/http.dart' as http;
import 'dart:convert';

class StorageMethods {
  final String cloudinaryUrl = "https://api.cloudinary.com/v1\_1/your-cloud-name/image/upload";
  final String cloudinaryPreset = "your-upload-preset";

  Future<String> uploadImageToStorage(
      bool isPost,
      String childName,
      Uint8List file,
  ) async {
    String uniqueId = const Uuid().v1();
    var uri = Uri.parse(cloudinaryUrl);
    var request = http.MultipartRequest('POST', uri);
    request.fields\['upload\_preset'\] = cloudinaryPreset;
    request.fields\['folder'\] = childName;
    request.fields\['public\_id'\] = isPost ? uniqueId : '';

    var multipartFile = http.MultipartFile.fromBytes('file', file, filename: '$uniqueId.jpg');
    request.files.add(multipartFile);

    var response = await request.send();
    if (response.statusCode == 200) {
      var responseData = await response.stream.toBytes();
      var jsonResponse = jsonDecode(String.fromCharCodes(responseData));
      return jsonResponse\['secure\_url'\];
    } else {
      throw Exception('Failed to upload image to Cloudinary');
    }
  }
}
```
Inside the `upload_image_screen.dart`:

Create a `StatefulWidget` Called `AddPicture` that accepts three arguments :

*   `final String email`
*   `final String password`
*   `final String username`

And contains a variable called `_image`

*   `Uint8List? _image`

Create two methods:

The first one is Called `selectImageFromGallery()`:

*   Prototype
    *   `void selectImageFromGallery()`
    *   Return the value to variable `_image`
*   Use `imagepicker`

the second one is Called `selectImageFromCamera()`:

*   Prototype
    *   `void selectImageFromCamera()`
    *   Return the value to variable `_image`
*   Use `imagepicker`

**Now**

Let’s Create this UI:

The [Link To the Icon](https://upload.wikimedia.org/wikipedia/commons/9/99/Sample_User_Icon.png "Link To the Icon")

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/12/6e67866cb45b4f9a5566e8bdd96434c994e93f85.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=11ef7e6926f62e3bcaadcdccfea57a6e55c385e18192f5af00e4b330dd6fc0e6)

Make the camera icon and the gallery icon linking with these functions

Replace the user icon with your image:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/12/b20daf8cf9cce7daef82cec6fb3e4170d6e81250.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f9a9719750bfb7d3d052822c4a6fe114b9f50660bcaef3e8dd5385f8ca8b29af)

  

### 9.

We are going to pass the sign up data to our upload picture page:

Inside `signup_screen.dart`

In the `onPressed` where the Text contain `Sign up`

use the `Navigator` to move to the `AddPicture` page and passing :

*   `email`
*   `username`
*   `password`

Inside `upload_image_screen.dart`:

**Use widget when you want to call the data example**:

`widget.email` or assign it to a variable `var email = widget.email`

Replace `John Doe` with the `username`

On the Next button call the method `signUpUser` that we created in the `auth_methods.dart`

Passing the correct data to the `signUpUser`

*   `email` takes `email`
*   `username` takes `username`
*   `password` takes `password`
*   `file` takes `_image`
*   on `success` show a `snackbar` with a `success` on it

  

### 10.

Create a new method called `getUserDetails` inside `auth_methods.dart` that gets the current user details and return `Userd.fromSnap` within the details

Inside the `lib/` create a new folder called `providers` that contain `user_provider.dart` file:

Inside `user_provider.dart` Create a class called `UserProvider` mixin with the `ChangeNotifier`

Create privet variables:

*   `_user` takes `Userd`
*   `_authMethode` takes `AuthMethode()`

Create a getter for `_user`

Create a method called `refreshUser` prototype:

*   Future refreshUser():
    *   `user` takes `getUserDetails` method from `AuthMethode()`
    *   `_userd` takes `user`
    *   at the end add `notifyListeners()`

  

### 11.

We are going to create the Home page now :

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/12/88520f0e2186e12e41d93b10cb312de6acc83bee.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=69dd96ae4a33301005e0e4a740b3f14e2ab0540d07115aeef0fbe6edcb37dc94)

**First** we are going to create all pages:

*   Create a new folder inside the screens folder called `Pages`:
    
    *   `Feed()` : `feed.dart`
    *   `Search()` : `search.dart`
    *   `AddImage()`: `add_image.dart`
    *   `Favorite()` : `favorite.dart`
    *   `Profile()` : `profile_screen.dart`

To start with the bottom navigation bar

Install this package:

*   [BottomNavyBar](/rltoken/nQ4YnR5B2dJLE_3MMrbhCQ "BottomNavyBar")

Inside the `widgets` folder:

*   Create a new file called `bottom_nav.dart`
    *   Create a `StatefulWidget` called `BottomNav`
    *   `_currentIndex` : `0`
    *   `_pageController` assign to `PageController`
    *   `initState()`:
        *   `_pageController` : PageController()
    *   `dispose()`
    *   Return `Scaffold`body `PageView`
        *   `controller` : `_pageController`
    *   `children` takes all the pages:
        *   `Feed()`
        *   `Search()`
        *   `AddImage()`
        *   `Favorite()`
        *   `Profile()`
    *   `bottomNavigationBar` : `BottomNavyBar`
        *   `selectedIndex` : `_currentIndex`
        *   `showElevation` : `true`
        *   `itemCornerRadius` : `8`
        *   `curve` : `Curves.easeInBack`
        *   `onItemSelected`: `onPageChanged` takes an arguments called index
            *   in `setState` `_currentIndex` takes `index`
    *   `items` it’s a list of `BottomNavyBarItem` we are going to create Five of them and every each one has a different `Icon` , `Text`:
        *   Inside `BottomNavyBarItem`:
        *   `icon`: `Icons`
        *   `title` : `Text`
            *   `TextStyle`:
                *   `fontSize` : `25`
                *   `fontFamily`: `Billabong`
            *   `activeColor` : `red`
            *   `textAlign`: `center`
            *   `inactiveColor`: `black`

**Now**

Inside `home.dart`

Create `StatefulWidget` called `Home` that returns `BottomNav()`

Inside `feed.dart`

Create `StatelessWidget` called `Feed` that returns `Scaffold()`:

*   With an `AppBar` contains `Holbegram` with `Billabong` font and the logo like in the Picture and a `Row` with two Icons
*   Body return widget called `Posts()` that we are going to create later

In the `models/post.dart`

*   Create a class called `Post`
    *   `caption` : `String`
    *   `uid`: `String`
    *   `username` : `String`
    *   `likes` : `List`
    *   `postId` : `String`
    *   `datePublished` : `DateTime`
    *   `postUrl` : `String`
    *   `profImage` : `String`

Create the instance `fromJson` like we did in the Users Class

Don’t forget the `toJson` method

Inside `utils/posts.dart`:

Create a `StatefulWidget` Called `Posts` using the `getUser`

**Use the provider and make necessary changes if required**

*   Return `StreamBuilder` :
    *   `stream` : `FirebaseFirestore.instance.collection('posts').snapshots()`
    *   if `snapshot.hasError` return `Error {snapshot.error}`
    *   if `snapshot.hasData` return `ListView.builder`
    *   `data` = `snapshot.data.docs`
        *   Return `SingleChildScrollView`
        *   `Child` : `Container`:
        *   `margin`: `EdgeInsetsGeometry.lerp(const EdgeInsets.all(8), const EdgeInsets.all(8), 10)`
        *   `height` : `540`
        *   `decoration`: `color fromARGB(255, 255, 255, 255), borderRadius circular(25)`
        *   `child` : `Column` > `children` > `Container` > `child` > `row` > `children`
            *   `padding EdgeInsets.all(8.0)` > `child` > `Container width: 40, height: 40,` > `decoration BoxDecoration(shape: BoxShape.circle)` > `image` > `data['profImage'] fit : cover`
            *   `Text` : `username`
            *   `Spacer`
            *   `IconButton`:
                *   `Icon` : `more_horiz`
                *   `onPressed` : Show snack with `Text` “Post Deleted”
            *   `SizedBox` :
                *   `child` : `Text` that contain the `caption`
            *   `SizedBox` :
                *   `height` : `10`
            *   `Container` :
                *   `width` : `350`
                *   `height` : `350`
                *   `decoration` : `BorderRadius.circular` `25`
                *   `image` : `postUrl`
                *   `fit` : `cover`

Add the missing `Icons` that appears in the `Picture`

Return `CircularProgressIndicator()` if the data still fetching

  

### 12.

Inside the `Pages` folder create a new folder called `methods`:

Inside the `methods` create a new file called `post_storage.dart`:

*   Create a class called `PostStorage`:
    *   `_firestore` takes : `FirebaseFirestore.instance`

**Methods**

Create a method Called `uploadPost` takes `caption`, `uid`, `username`, `profImage` as a `String` and `image` as `Uint8List`

*   Method prototype : `Future<String> uploadPost(String caption,String uid,String username,String profImage,Uint8List image)`

should use `uploadImageToCloudinary` from `lib\screens\auth\methods\user_storege.dart`

Return “`Ok`” On success else Return the error

Create another method called `deletePost` that accept `postId` and `publicId` as an arguments to delete the post

*   Method prototype : `Future<void> deletePost(String postId, string publicId)`

Inside `utils/posts.dart`:

*   In the `onPressed()` Before the `snackbar` that shows “Post Deleted” Call the the `deletePost` it should delete your post when you pressed on the icon

  

### 13.

Inside `add_image.dart` we are going to create this UI:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/12/ba9288292c9e3260060f022c7a40f0ef94f6ca7d.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f34e724e251cdd178e2b47a6c0ddd74cfedd0a1e4cb843dd4d16e962c31d4fea)

[Link to the Icon](https://cdn.pixabay.com/photo/2017/11/10/05/24/add-2935429_960_720.png "Link to the Icon ")

**Make necessary changes if required**

Like we did in the `AddPicture`

*   Use `image_picker`
    *   Using the two option to add an image \[`gallery`, `camera`\]

Call `uploadPost` when you press on `Post` and make sure to redirect to the `Home page`

  

### 14.

Inside `search.dart` we are going to create this UI:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/12/a22f19f7732ea369bbe4777e0a912e8948b214b4.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ac9a156706790c282ee0e0fa0451105d954f06a78b7196c9b71808e83454efd1)

**Make necessary changes if required**

*   Display all images uploaded to `Cloudinary`.
*   Use `StaggeredGridView`

  

### 15.

Inside `favorite.dart` we are going to create this UI:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/12/e8c14474c9b6315cb5aeff9616b7f5fe9b0054e2.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=73896f2b807954a7b62914b4bad383383c615e336bdf6aa7c82e4c6f49f7ca31)

**Make necessary changes if required**

when clicking on the `Icons.bookmark` in the Feed the image get saved and it appears in the Favorite page

  

### 16.

Inside `profile.dart` we are going to create this UI:

![](https://s3.eu-west-3.amazonaws.com/hbtn.intranet/uploads/medias/2022/12/cb96776b56e542882e5d58b85d19be6869754c5e.jpg?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIA4MYA5JM5DUTZGMZG%2F20250718%2Feu-west-3%2Fs3%2Faws4_request&X-Amz-Date=20250718T074319Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=fcb8fe583429dde57338ea3b79af30982c5fb34a469fe92a1f987f0f3ceeae05)

The icon at the top is for Logout.

**Make necessary changes if required**

Retrieve and display the necessary data, including images stored on Cloudinary.

And **congratulations** you made it