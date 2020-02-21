# Common command lines
### build / run
ionic cordova run android / ios --device -lcs # live reload - l = live, c = console
ionic cordova build android / ios

### list of devices
adb devices # real devices & simulator devices

# Debug
### Chrome
`chrome://devices` -> select `inspect`

# Issues
### no search file or directory, open: `...app-debug.apk`
`ln ./platforms/android/build/outputs/apk/android-debug.apk ./platforms/android/app/build/outputs/apk/debug/app-debug.apk`
