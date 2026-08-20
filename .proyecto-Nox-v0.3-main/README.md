# Proyecto Nox v0.2

Proyecto Android de Nox, preparado para compilación mediante GitHub Actions.

## Estructura corregida

El módulo Android utiliza la estructura estándar:

- `app/build.gradle.kts`
- `app/src/main/AndroidManifest.xml`
- `app/src/main/java/...`
- `app/src/main/res/...`
- `app/src/main/assets/...`
- `app/src/test/...`
- `app/src/androidTest/...`
- `gradle/libs.versions.toml`
- `gradle/wrapper/gradle-wrapper.properties`

El workflow `.github/workflows/android.yml` usa JDK 17 y el Gradle Wrapper.

## Compilación

GitHub Actions ejecuta:

`./gradlew assembleDebug`

y publica el APK como artifact `Nox-debug-apk`.
