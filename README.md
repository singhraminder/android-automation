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
6. Start Appium
```
C:\Users\singh>appium
[Appium] Welcome to Appium v2.12.1
[Appium] The autodetected Appium home path: C:\Users\singh\.appium
[Appium] Appium REST http interface listener started on http://0.0.0.0:4723
[Appium] You can provide the following URLs in your client code to connect to this server:
        http://192.168.56.1:4723/
        http://192.168.1.18:4723/
        http://127.0.0.1:4723/ (only accessible from the same host)
        http://172.23.144.1:4723/
[Appium] No drivers have been installed in C:\Users\singh\.appium. Use the "appium driver" command to install the one(s) you want to use.
[Appium] No plugins have been installed. Use the "appium plugin" command to install the one(s) you want to use.
```
