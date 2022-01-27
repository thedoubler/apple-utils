#  
# iOS Simulator - Command Line tools

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

# iOS Device - Secret Codes

Go to Phone numpad and type, then hit call:


#### Field Test Menu -
info about: Bandwith, PLMN (Public Land Mobile Network), RSRP (Reference Signal Received Power) -90 means good signal, Cell ID, EARFCN etc.
```
*3001#12345#* 
```

#### Call Barring 
disable/enable all incoming calls 

```
*#33# (Check status) 
*33*pin# (Enable Call Barring)
#33*pin# (Call Barring)

_pin is which is the lock on your SIM card._
```

#### Call Forwarding 
disable/enable all incoming calls 

*#21# (check status)
*21# (enable/disable Call Forwarding)
*21mobilenumber# (divert calls to Number)
