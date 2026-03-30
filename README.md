📖 About
BuildQcheck (BuildZone QA Monitor) is a comprehensive Android application designed for construction field workers and site managers. It enables real-time quality inspections, issue reporting, material compliance checks, and site progress tracking — all backed by Firebase Firestore.

✨ Features
FeatureDescription🔐 AuthenticationEmail/password login, signup, forgot password, and email verification via Firebase Auth🏠 Home DashboardQuick-access grid to Add Site, Site List, Feedback, and About📋 Site ManagementAdd, update, and track construction sites (Residential / Commercial / Industrial)✅ Quality CheckRadio-group-based quality quiz evaluating Bricks, Steel, Concrete, Waterproofing, Wiring, Plaster, and Fire Door Rating⚠️ Report IssuesLog safety/quality issues with category dropdown and description — saved to Firestore📊 Site DetailsFull site info view with colour-coded status (Active / Completed / To Start)📚 Materials InfoReference standards (IS 456:2000, NBC 2016) via popup windows for each material category💬 FeedbackStar rating + text feedback submitted to Firebase👤 ProfileView account info, sign out, and delete account

🗂️ App Navigation
HomeScreen
├── AddSiteScreen          → Register a new construction site
├── SiteListScreen         → View all ongoing sites
│   └── SiteDetailsScreen  → Site overview + colour-coded status
│       ├── SiteActionsScreen
│       │   ├── CheckQualityScreen  → Run material quality quiz
│       │   └── ReportIssueScreen   → Log issues/safety concerns
│       └── (Update site info)
├── MaterialInfoFragment   → Reference standards (Concrete, Steel, Bricks, Wiring, Waterproofing, Plaster, Fire Safety)
├── FeedbackScreen         → Submit star rating + comments
├── AboutScreen            → App info and developer contact
└── ProfileFragment        → Account management

🛠️ Tech Stack

Language: Kotlin
UI: XML Layouts, View Binding
Architecture: Activity + Fragment based
Backend: Firebase Firestore, Firebase Authentication
Other: RecyclerView, PopupWindow, Toast, ArrayAdapter (Spinner)


🚀 Getting Started
Prerequisites

Android Studio Flamingo or newer
Android SDK 24+
A Firebase project with Firestore and Authentication enabled

Setup

Clone the repository

bash   git clone https://github.com/YOUR_USERNAME/BuildQcheck.git
   cd BuildQcheck

Add Firebase config

Go to Firebase Console
Create a project → Add an Android app with package com.example.bqc
Download google-services.json and place it in the /app directory


Enable Firebase services
Firebase Authentication → Email/Password provider
Cloud Firestore → Start in test mode
Open in Android Studio
Sync Gradle
Run on emulator or physical device (API 24+)

📁 Project Structure
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

🔥 Firebase Collections
firestore/
├── sites/
│   └── {documentID}
│       ├── name, description, materialsUsed
│       ├── siteType, currentWork
│       ├── totalBudget, spendings
│       ├── startDate, endDate, siteStatus
│       └── qualityCheck (report string)
├── feedback/
│   └── {docID} → feedback (text), rating (int)
└── report/
    └── {docID} → category, description, userEmail









