# Set up a real mobile device for testing #34

## How do you enable developer mode on Android and iOS?

Android:  
Open Settings → About phone.  
Tap Build number seven times.  
Go back and open System → Developer options, then turn it on.  
  
iOS:  
On recent iOS versions:  
Install a development or TestFlight build of the app.  
On the iOS device, go Settings → Privacy & Security → Developer Mode.  
Tap Enable and confirm with your passcode.  

## What tools can you use to inspect and debug apps on a real device?
we can use tools like:
- Android studio with Logcat for Android
- Xcode + Console for ios 

## How do you capture logs from an Android/iOS device while testing?
Android:
- use Android Studio Logcat while the app runs, filter by app name, and save the log output
ios:
- connect device to a Mac with Xcode and open Devices & Simulators to view logs

## What are common challenges when testing on physical devices, and how do you work around them?
common challenges include:
- hardware variability
- network and location realism
- device management
To work around these:
- use cloud-device platforms for a mix of popular and older devices
- keep a small device library of key moddels for focuse testing

## What issues might only appear on a real device but not on an emulator?
issues like crashes from low memory or slow CPU on older phones, GPS or sensor inaccuracies, camera or microphone problems when using the real hardware.

## How would you report a bug that only happens on a specific device model?
I would clearly state in the title that it's device-specific, note the device name, OS version, app version, network, and battery level, describe the exact steps and any patterns, and attach logs, screenshots, or a short screen recording from the real device.

## If an app crashes on a physical device, what steps would you take to gather useful debugging information?
I would reproduce it once more and note the exact steps and conditions, capture logs, take screnshots or recording of the app just before the crash, record device details, and create clear bug report with environment, steps, log snippet, and impact.
