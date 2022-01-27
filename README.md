#  

iOS Simulator


Remove unavailable iOS Simulators

```
xcrun simctl delete unavailable
```

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

Add Media to iOS Simulator (or drag and drop)

```
xcrun simctl addmedia booted PATH_TO_MEDIA_FILE
```

Record a video from Simulator (⌘ + R)

```
xcrun simctl io booted recordVideo --type=mp4 PATH_TO_FILE
```
Use Simulator in Fullscreen MODE

```
defaults write com.apple.iphonesimulator AllowFullscreenMode -bool YES
```

Clean Derived Data (alias)

```
rm -rf ~/Library/Developer/Xcode/DerivedData
rm -frd ~/Library/Caches/com.apple.dt.Xcode/*
```

# iOS Device - Secret Menu
<details>
  <summary>Click to expand!</summary>
  
  ## Heading
  1. A numbered
  2. list
     * With some
     * Sub bullets
</details>

