# Caregiver App – Information Architecture

App --> Home[Home]
App --> Plan[Plan]
App --> Shop[Shop]
App --> Progress[Progress]
App --> Alerts[Alerts]
App --> Settings[Settings]
App --> Healbot[Healbot]

Home --> HomeMeals[Today's Meals]
Home --> HomeQuickLog[Quick Log Meals]
Home --> HomeHealthSnap[Health Snapshot]
HomeMeals --> HomeMealQuickView[Meal Quick View]
HomeMealQuickView --> HomeMealDetail[Meal Detail]

Plan --> PlanWeekly[Weekly View]
PlanWeekly --> PlanDaily[Daily Cards]
PlanDaily --> PlanMealDetail[Meal Detail]
PlanMealDetail --> PlanSwap[Swap Meal]
PlanWeekly --> PlanRegen[Regenerate Plan]

Shop --> ShopList[Shopping List]
ShopList --> ShopMode[Shopping Mode]
ShopMode --> ShopDone[Completion Overlay]

Progress --> ProgMeals[Meal Progress]
Progress --> ProgHealth[Health Progress]

ProgMeals --> ProgWeekSummary[Week Summary]
ProgMeals --> ProgHeatmap[Heatmap]
ProgMeals --> ProgDayDetail[Day Detail]
ProgMeals --> ProgAchievements[Achievements]

ProgHealth --> ProgQuickLog[Quick Log Cards]
ProgHealth --> ProgSummary[Today's Summary]
ProgHealth --> ProgTrends[Trends]
ProgTrends --> ProgExport[Export Data]

Alerts --> AlertsActive[Active Alerts]
Alerts --> AlertsHistory[Alert History]

Settings --> SetProfile[Profile]
Settings --> SetTargets[Health Targets]
Settings --> SetAlertPrefs[Alert Preferences]
Settings --> SetContacts[Emergency Contacts]
Settings --> SetData[Data Export]
