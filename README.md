📂 DocSaver – Secure Cloud Document Manager

DocSaver is a Flutter application that lets users securely upload, view, and manage their important documents like PDFs and images. Built using Firebase for authentication, real-time database, and cloud storage, it’s designed with simplicity, speed, and security in mind.

🚀 Features:

🔐 User Authentication
Login & Register with Email and Password
Password reset via email
Secure Firebase Authentication

📁 Document Upload & Viewing
Upload PDFs and images
View documents inside the app (using flutter_pdfview and Image.file)
Smart UI to show file types visually
File preview with metadata: title, type, and upload date

🧠 Intelligent Search
Real-time search from Firebase Realtime Database
Search by document title with instant results

⚙️ User Profile & Settings
Update username
View email
Logout securely
Delete account (with all user data and storage cleanup)

🌈 Smooth UI/UX
Consistent theming using custom buttons and fields
Gradient backgrounds and clean layout

🛠️ Tech Stack:
DocSaver uses modern tools and technologies to build a seamless, cloud-integrated Flutter application:

⚙️ Frontend – Flutter
Cross-platform mobile framework used to build the UI/UX of the app.
Language: Dart
UI Framework: Flutter
State Management: Provider
Widgets:
CustomTextField, CustomButton, CustomFloatingActionButton – Reusable and stylized widgets
ScreenBackgroundWidget – Consistent screen backgrounds with gradient
FileCard – UI component to display each document visually
Routing: Named routes using MaterialApp.routes

🔥 Backend – Firebase
Firebase is used to handle authentication, database, and file storage.
1. Firebase Authentication
Email/Password Sign-In
Password Reset
Account creation and deletion
Securely handles session and user identity

2. Firebase Realtime Database
Stores document metadata (title, fileName, fileUrl, dateAdded, fileType, etc.)
Real-time streaming using StreamController and .onValue
Supports live search using startAt() and endAt() with Unicode wildcard (\uf8ff)

3. Firebase Storage
Upload and store PDF and image files
File retrieval for viewing or downloading
Linked with Realtime Database entries

4)Packages Used:

firebase_core: Initialize Firebase in the app
firebase_auth: Handle user authentication
firebase_database: Store and stream document data
firebase_storage: Upload and fetch files from cloud storage
provider: State management
flutter_pdfview: Render and display PDF files
path_provider: Save/download files to local storage
http: Download files using HTTP GET

Testing & Debugging:
Hot reload via Flutter DevTools
print and snackbar-based error feedback
Loading indicators (custom progress widgets during API calls)
