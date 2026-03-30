BuildQCheck is a comprehensive Android application designed for construction field workers and site managers.
It enables quality inspections, issue reporting, material compliance checks, and site progress tracking.

#Features
🔐 Authentication
Email/password login & signup
Forgot password support
Email verification using Firebase Authentication
#🏠 Dashboard
Grid-based home screen for quick navigation
Access to key modules: Add Site, Site List, Feedback, About
📋 Site Management
Add, update, and manage construction sites
Supports Residential / Commercial / Industrial categories
#✅ Quality Check
Interactive radio-based quality assessment quiz
Covers:
Bricks
Steel
Concrete
Waterproofing
Wiring
Plaster
Fire Door Rating
#⚠️ Issue Reporting
Log safety or quality issues
Category-based dropdown + detailed description
Data stored in Firebase Firestore
#📊 Site Details
Detailed site overview
Status indicators:
🟢 Active
🔵 Completed
🟡 To Start
📚 Material Reference
#💬 Feedback System
Star rating + user comments
Stored in Firebase
#👤 Profile Management
View account details
Logout and delete account

#🗂️ App Navigation
HomeScreen
├── AddSiteScreen          → Register new site
├── SiteListScreen         → View all sites
│   └── SiteDetailsScreen  → Detailed site info
│       ├── SiteActionsScreen
│       │   ├── CheckQualityScreen
│       │   └── ReportIssueScreen
│       └── Update Site Info
├── MaterialInfoFragment   → Standards reference
├── FeedbackScreen         → Submit feedback
├── AboutScreen            → App info
└── ProfileFragment        → Account management

#🛠️ Tech Stack
Language: Kotlin
UI: XML Layouts, View Binding
Architecture: Activity + Fragment-based
Backend: Firebase Firestore, Firebase Authentication
Libraries & Components:
RecyclerView
PopupWindow
Toast
ArrayAdapter (Spinner)

#🚀 Getting Started
#🔧 Prerequisites
Android Studio (Flamingo or newer)
Android SDK 24+
Firebase project with Firestore & Authentication

#📁 Project Structure
app/src/main/java/com/example/bqc/
├── SplashScreen.kt
├── SignIn.kt
├── SignUp.kt
├── ForgotPassword.kt
├── MainActivity.kt
├── homefragment.kt
├── materialinfofragment.kt
├── profilefragment.kt
├── AddSite.kt
├── SiteList.kt
├── SiteDetails.kt
├── SiteActions.kt
├── QualityQuiz.kt
├── ReportIssues.kt
├── Feedback.kt
└── AboutScreen.kt




