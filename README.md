Description

Companion Hub is a cross-platform iOS Android companion app providing wallet, authentication, purchase flow, and health integration. As Mobile Team Lead, targets:

Session retention: ≥ 75% at 30 days

App size: ≤ 50 MB

Key features:

Languages & Frameworks: Swift 5.9 (iOS 17), Kotlin 1.9 (Android 15)

UI: SwiftUI / Jetpack Compose

Networking: GraphQL via Apollo client

Crash Reporting: Firebase Crashlytics

Security: FIDO2 authentication fallback

Payments: In‑app purchase flow (StoreKit / Play Billing)

Health Data: HealthKit bridge / Google Fit integration

Fallback: Heavy inference fallback (on-device ML via Core ML / TensorFlow Lite)

CompanionHub/
├── README.md
├── ios/
│   ├── CompanionHub.xcodeproj
│   ├── App/  
│   │   ├── Assets.xcassets
│   │   ├── App.swift
│   │   ├── Views/
│   │   │   ├── HomeView.swift
│   │   │   ├── WalletView.swift
│   │   │   ├── AuthView.swift
│   │   │   └── HealthBridgeView.swift
│   │   ├── Models/
│   │   ├── Services/
│   │   │   ├── GraphQLService.swift
│   │   │   ├── AuthService.swift
│   │   │   ├── PurchaseService.swift
│   │   │   └── HealthService.swift
│   │   └── Utilities/
│   │       └── CrashlyticsConfigurator.swift
│   └── Podfile
├── android/
│   ├── app/
│   │   ├── src/main/
│   │   │   ├── java/com/yourorg/companionhub/
│   │   │   │   ├── MainActivity.kt
│   │   │   │   ├── ui/
│   │   │   │   │   ├── HomeScreen.kt
│   │   │   │   │   ├── WalletScreen.kt
│   │   │   │   │   ├── AuthScreen.kt
│   │   │   │   │   └── HealthBridgeScreen.kt
│   │   │   │   ├── data/
│   │   │   │   └── service/
│   │   │   │       ├── GraphQLClient.kt
│   │   │   │       ├── AuthService.kt
│   │   │   │       ├── PurchaseService.kt
│   │   │   │       └── HealthService.kt
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle.kts
│   └── settings.gradle.kts
└── shared/
    ├── graphql/
    │   └── schema.graphqls
    └── ml/
        ├── Model.mlmodel
        └── model.tflite
