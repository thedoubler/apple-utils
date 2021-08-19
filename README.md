#  

iOS Simulator

Get iOS Simulator *.app **file** 

```
xcrun simctl get_app_container booted your.bundle.identifer
```
Get iOS Simulator *.app **data**
```
xcrun simctl get_app_container booted your.bundle.identifer data
```

Get iOS app info 

```
xcrun simctl appinfo booted your.bundle.identifer
```

Launch the app in iOS Simulator using command line args

```
xcrun simctl launch --console booted your.bundle.identifer "your -arguments"
```

Record a video from Simulator ⌘ + R

```
xcrun simctl io booted recordVideo --type=mp4 PATH_TO_FILE
```
