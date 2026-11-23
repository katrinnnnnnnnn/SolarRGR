# SolarGrid РГР (варіант 3: сонячна електростанція)

Android, Kotlin 2.0, Jetpack Compose, MVVM, Room, Retrofit, Flow, Navigation. minSdk 24, targetSdk 34.

## Перший запуск
1. Відкрити теку в Android Studio (File → Open). Studio завантажить Gradle 8.9 і залежності.
2. Для запуску з термінала згенерувати wrapper: `brew install gradle && gradle wrapper --gradle-version 8.9`
   (або просто виконати Sync у Android Studio — вона також створить gradlew).
3. `./gradlew installDebug` і `adb shell am start -n ua.kpi.solarrgr/.MainActivity`

Тести: `./gradlew testDebugUnitTest`, `./gradlew connectedDebugAndroidTest`.

Вхід: admin@solar.test / solar1234 (ADMIN); будь-який інший email із цим паролем — VIEWER.
Телеметрія симульована; токен — навчальна імітація, не JWT.
