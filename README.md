# GIMICI-web3
all Cotrol web3
Using npm:

npm install --save web3-react-native
Using yarn:

yarn add web3-react-native
For versions less than React Native 0.60, be sure to execute react-native link to make the native library dependencies visible to your compiled application.

iOS
After installing, append the following lines to your app's ios/Podfile, then execute pod install:

# web3-react-native
pod 'secp256k1.c', '0.1.2', :modular_headers => true
pod 'web3swift', '2.2.1', :modular_headers => true
⚠️ This is an ugly workaround for existing definition constraints in the Podspec. (View Issue).

Android
In your app's AndroidManifest.xml, you need to enable android:largeHeap under the <application> tag:

  <application
+   android:largeHeap="true"
  />
Perform a rebuild of your compiled application by calling react-native run-android.

For usage details, please see the
