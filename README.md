# חיפושי מדיה (Media Search)
אפליקציית Android (Kotlin + Jetpack Compose) לחיפוש סרטים, סדרות ושחקנים באמצעות TMDB.

## קבלת מפתח TMDB (API Key)
1. הירשם בחינם ב-https://www.themoviedb.org/signup
2. Settings → API → Create → Developer, ומלא את הטופס.
3. העתק את "API Key (v3 auth)" (או את ה-"API Read Access Token").
4. בשורש הפרויקט פתח/צור את הקובץ `local.properties` והוסף שורה:
   `TMDB_API_KEY=המפתח_שלך`
   (הקובץ ב-.gitignore ולכן לא יעלה ל-Git. ראה local.properties.example)
5. Sync Gradle ← Build.

## בנייה והתקנה
- פתח את התיקייה ב-Android Studio (Koala ומעלה, JDK 17), חכה ל-Sync (יוצר את ה-Gradle Wrapper).
- Build → Build APK(s). הקובץ: `app/build/outputs/apk/debug/app-debug.apk`
- העתק לטלפון (או חבר ב-USB עם Run) והתקן. נדרש Android 8.0+.
