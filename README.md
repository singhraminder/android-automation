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
7. Check drivers
```
C:\Users\singh>appium driver list
✔ Listing available drivers
- uiautomator2 [not installed]
- xcuitest [not installed]
- espresso [not installed]
- mac2 [not installed]
- windows [not installed]
- safari [not installed]
- gecko [not installed]
- chromium [not installed]
```
8. Install 3 drivers > uiautomator2, windows and chromium
```
C:\Users\singh>appium driver install uiautomator2
✔ Checking if 'appium-uiautomator2-driver' is compatible
✔ Installing 'uiautomator2' using NPM install spec 'appium-uiautomator2-driver'
ℹ Driver uiautomator2@3.8.0 successfully installed
- automationName: UiAutomator2
- platformNames: ["Android"]

C:\Users\singh>appium driver install windows
✔ Checking if 'appium-windows-driver' is compatible
✔ Installing 'windows' using NPM install spec 'appium-windows-driver'
ℹ Driver windows@3.0.2 successfully installed
- automationName: Windows
- platformNames: ["Windows"]

C:\Users\singh>appium driver install chromium
✔ Checking if 'appium-chromium-driver' is compatible
✔ Installing 'chromium' using NPM install spec 'appium-chromium-driver'
ℹ Driver chromium@1.4.4 successfully installed
- automationName: Chromium
- platformNames: ["Windows","mac","macOS","Linux"]
```
9. Install plugins > images
```
C:\Users\singh>appium
[Appium] Welcome to Appium v2.12.1
[Appium] The autodetected Appium home path: C:\Users\singh\.appium
[Appium] Attempting to load driver uiautomator2...
[Appium] Attempting to load driver windows...
[Appium] Attempting to load driver chromium...
[Appium] Requiring driver at C:\Users\singh\.appium\node_modules\appium-windows-driver\build\index.js
[Appium] Requiring driver at C:\Users\singh\.appium\node_modules\appium-chromium-driver\index.js
[Appium] Requiring driver at C:\Users\singh\.appium\node_modules\appium-uiautomator2-driver\build\index.js
[Appium] WindowsDriver has been successfully loaded in 3.604s
[Appium] ChromiumDriver has been successfully loaded in 3.604s
[Appium] AndroidUiautomator2Driver has been successfully loaded in 3.605s
[HTTP] Could not start REST http interface listener. The requested port may already be in use. Please make sure there is no other instance of this server running already.
[Appium] Could not configure Appium server. It's possible that a driver or plugin tried to update the server and failed. Original error: listen EADDRINUSE: address already in use 0.0.0.0:4723
[Appium] Error: listen EADDRINUSE: address already in use 0.0.0.0:4723
    at Server.setupListenHandle [as _listen2] (node:net:1872:16)
    at listenInCluster (node:net:1920:12)
    at doListen (node:net:2069:7)
    at processTicksAndRejections (node:internal/process/task_queues:83:21)

C:\Users\singh>appium plugin
Error: ✖ Cannot handle plugin command undefined

C:\Users\singh>appium plugin list
✔ Listing available plugins
- images [not installed]
- execute-driver [not installed]
- relaxed-caps [not installed]
- universal-xml [not installed]

C:\Users\singh>appium plugin install images
✔ Checking if '@appium/images-plugin' is compatible
✔ Installing 'images' using NPM install spec '@appium/images-plugin'
ℹ Plugin images@3.0.21 successfully installed
```
