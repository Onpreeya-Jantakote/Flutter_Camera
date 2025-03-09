# Flutter Camera App

A simple Flutter app demonstrating the use of the camera and image picker functionalities. The app allows users to capture photos using the device camera and view them in a gallery.

---

## 📸 Features
- Capture photos using the device's camera.
- Switch between front and rear cameras.
- Display captured photos in a gallery grid.
- View full-screen images when tapping on a photo.

---

## 🛠️ Installation

### 1. **Install Dependencies**
```bash
flutter pub get
```

### 2. **Add Required Packages**
```bash
flutter pub add camera
flutter pub add image_picker
flutter pub add permission_handler
```

### 3. **Configure Android Permissions**
Add the following permissions to `android/app/src/main/AndroidManifest.xml`:

```xml
    <uses-permission android:name="android.permission.CAMERA"/>
    <uses-feature android:name="android.hardware.camera" />
    <uses-feature android:name="android.hardware.camera.autofocus" />
    <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE"/>
    <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE"/>
    <uses-permission android:name="android.permission.READ_MEDIA_IMAGES"/>
```

### 4. **Build APK for Android**
To build the app into an APK file, use:
```bash
flutter build apk --release
```
The APK file will be generated in `build/app/outputs/flutter-apk`.

---

## 🎯 How to Use
- Tap the camera icon to open the camera interface.
- Switch between front and rear cameras using the switch button.
- Capture a photo by tapping the camera button.
- Captured photos will be displayed in the gallery.
- Tap any photo to view it in full-screen mode.

---

## 🚀 Dependencies
- **camera**: Provides access to the device camera.
- **image_picker**: Allows picking images from the gallery or camera.
- **permission_handler**: Manages runtime permissions.
