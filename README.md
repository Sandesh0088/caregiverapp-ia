# Caregiver App - Information Architecture

Complete screen hierarchy and navigation structure for meal planning + health tracking app for seniors.

%% Entry
A --> B[Splash/Loading]
B --> C[Auth]
C --> C1[Login]
C --> C2[Create Account]
C1 --> D[Home]
C2 --> E[Onboarding]
E --> E1[Add Mum Profile]
E1 --> E2[Health Conditions]
E2 --> E3[Generate Plan]
E3 --> D

%% Main Navigation (Bottom Tabs)
D --> F[Home]:::primary
D --> G[Plan]:::primary
D --> H[Shop]:::primary
D --> I[Progress]:::primary

%% Global/Secondary
D -.-> J[Alerts]:::secondary
D -.-> K[Settings]:::secondary
D -.-> L[Healbot]:::secondary

%% Home screens
F --> F1[Today's Meals Cards]
F1 --> F2[Meal Quick View]
F2 --> F3[Meal Detail]
F --> F4[Quick Log Meals Modal]
F --> F5[Health Snapshot]

%% Plan screens
G --> G1[Weekly View]
G1 --> G2[Daily Cards]
G2 --> G3[Meal Detail]
G3 --> G4[Swap Meal]
G1 --> G5[Regenerate Plan Modal]

%% Shop screens
H --> H1[Shopping List]
H1 --> H2[Shopping Mode]
H2 --> H3[Completion Overlay]

%% Progress screens
I --> I1[Progress Landing<br/>Meals|Health Tabs]
I1 --> I2[Meal Progress]
I2 --> I2a[Week Summary]
I2a --> I2b[Heatmap]
I2b --> I2c[Day Detail Modal]
I2 --> I2d[Achievements]
I1 --> I3[Health Progress]
I3 --> I3a[Quick Log Cards]
I3a --> I3b[Log Modal]
I3 --> I3c[Today's Summary]
I3 --> I3d[Trends Accordions]
I3d --> I3e[Export Data]

%% Alerts hierarchy
J --> J1[Active Alerts]
J1 --> J2[Alert Detail]
J --> J3[Alert History]

%% Settings hierarchy
K --> K1[Profile]
K --> K2[Health Targets]
K --> K3[Alert Preferences]
K --> K4[Emergency Contacts]
K --> K5[Data Export]

%% Overlay alerts (interrupt anywhere)
A -.-> AL1[Tier 1 Banner]
A -.-> AL2[Tier 2 Modal]
A -.-> AL3[Tier 3 Full Screen]
AL3 --> AL4[Senior: Call 999<br/>OR Rest+Retest]
AL3 -.-> AL5[Caregiver: Urgent Push]

%% Styling
classDef app fill:#e3f2fd,stroke:#1976d2,stroke-width:4px
classDef primary fill:#f3e5f5,stroke:#9c27b0,stroke-width:3px
classDef secondary fill:#fff3e0,stroke:#f57c00,stroke-width:2px
classDef modal fill:#f1f8e9,stroke:#689f38,stroke-width:2px
classDef alert fill:#ffebee,stroke:#d32f2f,stroke-width:3px

class A app
class F,G,H,I primary
class J,K,L secondary
class F2,F4,I2c,I3b,G4,G5,H3 modal
class AL1,AL2,AL3,AL4,AL5 alert
