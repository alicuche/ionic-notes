# Common command lines
### build / run
ionic cordova run android / ios --device -lcs # live reload - l = live, c = console
ionic cordova build android / ios

### list of devices
adb devices # real devices & simulator devices

# Debug
### Android / Chrome
![image](https://i.imgur.com/2P7LzV6.png)
### IOS / Safari
![image](https://i.imgur.com/FKkXT3K.jpg)


# Issues
### no search file or directory, open: `...app-debug.apk`
`ln ./platforms/android/build/outputs/apk/android-debug.apk ./platforms/android/app/build/outputs/apk/debug/app-debug.apk`

### xcode
1. xcode-select
xcode-select: error: tool 'xcodebuild' requires Xcode, but active developer directory '/Library/Developer/CommandLineTools' is a command line tools instance

`sudo xcode-select -s /Applications/Xcode.app/Contents/Developer`

2. /usr/local/bin/node
dyld: Library not loaded: /usr/local/opt/icu4c/lib/libicui18n.63.dylib
  Referenced from: /usr/local/bin/node
  Reason: image not found
  
`brew upgrade npm`

3. ios version
Error: Cannot read property 'toLowerCase' of undefined
[ERROR] An error occurred while running subprocess cordova.

```
cordova platform rm ios
cordova platform add ios@5.1.1
```

4. cordova version
[ERROR] An error occurred while running subprocess cordova.
cordova platform add ios exited with exit code 1.

`npm install -g cordova@8.1.2`
