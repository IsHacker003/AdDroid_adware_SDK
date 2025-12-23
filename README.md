# AdDroid adware SDK
This is an SDK for [AdDroid adware](https://github.com/IsHacker003/AdDroid_adware_standalone), which helps to integrate the adware into legitimate apps for penetration testing purposes.
## Compilation
Your app needs to have minSdk >= 23 to use this SDK. Just add the dependency, the adware will do everything automatically.

For `build.gradle`:
```
implementation (project(path: ":AdDroid-adware")) {
    transitive = true
}
```
For `build.gradle.kts`:
```
implementation(project(":AdDroid-adware")) {
    transitive = true
}
```
Also add this in `settings.gradle`:
```
include ':AdDroid-adware'
```
Optionally, your app should request location, notification and display over other apps permissions. If you do not request these permissions, the victim will have to manually grant them from the app info.

**For educational purposes only. Do not use for illegal purposes.**
