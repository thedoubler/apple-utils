#  

iOS Simulator

Get iOS Simulator *.app **file** 

```
xcrun simctl get_app_container booted *insert.bundle.identifer*
```
Get iOS Simulator *.app **data**
```
xcrun simctl get_app_container booted *insert.bundle.identifer* data
```

Get iOS app info 

```
xcrun simctl appinfo booted *insert.bundle.identifer*
```

Launch the app in iOS Simulator using command line args

```
xcrun simctl launch --console booted *insert.bundle.identifer* "your -arguments"
```

Record a video from Simulator ⌘ + R

```
xcrun simctl io booted recordVideo --type=mp4 PATH_TO_FILE
```
