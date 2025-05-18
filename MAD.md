
# 📱 Mobile Application Development

## 📌 Overview
Mobile Application Development involves creating software applications that run on a mobile device. It includes native apps for Android, iOS, Windows, and hybrid apps using HTML5. This field is rapidly growing due to the widespread use of smartphones and tablets.

---

## 🛠 Mobile Application Development Platforms

### 🔹 HTML5 for Mobiles
- Enables cross-platform mobile app development.
- Responsive layout, offline support, and access to device features using frameworks like PhoneGap/Cordova.

---

## 🤖 Android OS

### 🧱 Architecture
- **Linux Kernel**: Core system services and hardware abstraction.
- **Libraries & Runtime**: Includes ART (Android Runtime), core libraries.
- **Application Framework**: System services like Activity Manager, Window Manager.
- **Applications**: User apps on top of the stack.

### 🧰 Framework & Application Development
- Uses **Java/Kotlin** for native apps.
- Structured around `Activities`, `Fragments`, `Services`, `Broadcast Receivers`, and `Content Providers`.

---

## 🍏 iOS

### 🧱 Architecture
- **Core OS**: Kernel, low-level features.
- **Core Services**: Networking, databases.
- **Media**: Audio, video, graphics.
- **Cocoa Touch**: UI, event handling.

### 🧰 Framework
- Developed using **Swift** or **Objective-C**.
- Xcode IDE for UI design and coding.

---

## 🪟 Windows Mobile Development
- Previously supported by **Visual Studio** using **C#** and **.NET Compact Framework**.
- Limited market share today, but important historically.

---

## 🧩 Fragments
- Modular sections of an Activity.
- Reusable and adaptable to screen sizes and orientation changes.

---

## 📞 Calling Built-in Applications using Intents

Use `Intent` class to interact with native apps (dialer, camera, SMS, etc.):

```kotlin
val intent = Intent(Intent.ACTION_DIAL, Uri.parse("tel:123456789"))
startActivity(intent)
```

---

## 🔔 Displaying Notifications
Notify users of important events using `NotificationManager` and `NotificationCompat`.

---

## 📺 Components of a Screen
Includes `TextView`, `EditText`, `Button`, `ImageView`, `RecyclerView`, etc.

---

## 📲 Adapting to Display Orientation
Use `onConfigurationChanged()` and resource folders (`layout-land`, `layout-port`) to manage layouts.

---

## 🔄 Managing Screen Orientation Changes
Prevent activity restart using:

```xml
android:configChanges="orientation|screenSize"
```

---

## 🎛 Utilizing the Action Bar
Use for navigation, branding, and user actions.

---

## 🧑‍🎨 Creating the User Interface
Built with XML layouts and Kotlin/Java. Supports themes, styles, and dynamic UI changes.

---

## 👂 Listening for UI Notifications
Use event listeners like `onClickListener`, `onTextChanged`, etc.

---

## 🪟 Views
Basic building blocks: `View`, `ViewGroup`, `TextView`, `Button`, `ImageView`, etc.

---

## ⚙ User Preferences
Store key-value pairs using `SharedPreferences`.

---

## 🗂 Persisting Data
Use `SQLite`, `Room`, `SharedPreferences`, or internal storage.

---

## 🔗 Sharing Data
`Content Providers` allow apps to share data securely.

---

## 💬 Sending SMS Messages

```kotlin
val smsIntent = Intent(Intent.ACTION_SENDTO, Uri.parse("smsto:123456789"))
smsIntent.putExtra("sms_body", "Hello!")
startActivity(smsIntent)
```

---

## ✅ Getting Feedback
Use dialogs, toasts, snackbars, or haptic feedback.

---

## 📧 Sending Email

```kotlin
val intent = Intent(Intent.ACTION_SEND)
intent.type = "message/rfc822"
intent.putExtra(Intent.EXTRA_EMAIL, arrayOf("example@gmail.com"))
intent.putExtra(Intent.EXTRA_SUBJECT, "Subject")
intent.putExtra(Intent.EXTRA_TEXT, "Body")
startActivity(Intent.createChooser(intent, "Send Email"))
```

---

## 🗺 Displaying Maps
Use Google Maps SDK for Android or iOS.

---

## 🌐 Consuming Web Services Using HTTP
Use `Retrofit`, `Volley`, or `HttpURLConnection` for RESTful API calls.

---

## 🧠 Web Services: Accessing & Creating
- Backend services: Flask, Django, Node.js.
- Access via HTTP: `GET`, `POST`, `PUT`, `DELETE`.

---

## 🧵 Threading
Use `AsyncTask`, `Handler`, or `Coroutines` for background tasks.

---

## 🚀 Publishing Android Applications
- Generate signed APK or AAB.
- Upload to Play Store with description, screenshots, and app info.

---

## 🏬 Deployment on App Stores
- iOS: App Store Connect.
- Android: Google Play Console.
- Windows: Microsoft Store Developer Center.

---

## 🔤 Mobile Programming Languages
- **Android**: Java, Kotlin
- **iOS**: Swift, Objective-C
- **Hybrid**: HTML5, JavaScript (React Native, Flutter)

---

## ⚠ Challenges with Mobility & Wireless Communication
- Network reliability
- Data security
- Device compatibility
- Battery constraints

---

## 📍 Location-aware Applications
Use GPS, Network Providers, and Google Location Services for real-time location tracking.

---

## ⚖ Performance/Power Tradeoffs
Optimize background tasks, reduce battery usage, and minimize network calls.

---

## 📱 Mobile Platform Constraints
- Limited screen size
- Limited memory and battery
- Hardware fragmentation

---

## 🚀 Emerging Technologies
- AR/VR
- AI-powered apps
- IoT integration
- 5G support
- Wearables

---

## 📢 License
This project/documentation is part of educational material. Feel free to reuse with attribution.
