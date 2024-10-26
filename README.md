# android-automation
android app functional automation using appium

1. Installed new Android-Studio LadyBug (2024.2.1) on 26.Oct.2024
2. Within Android Studio Settings > Settings > Build Tool > Gradle is not pointed to wrapper but points to local installation / distribution (GRADLE_HOME) and JDK is pointed to JDK_HOME
3. Installed new gradle version > 8.10.2 and make sure GRADLE_HOME is point to C:\sw.1\gradle-8.10.2 as well in Advanced Settings > env variables i.e. PATH also points to %GRADLE_HOME%\bin
4. Check node and npm versions
```
> node -v
v20.7.0
> npm -v
10.1.0
//upgrade npm
> npm install -g npm@10.9.0
> npm -v
10.9.0
```
5. Install appium
```
> npm install -g appium
```
