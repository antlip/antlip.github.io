---
layout: post
title: Two ways to create an Android Virtual Device in Android Studio 4.1.1
subtitle: Learn how to create an Android Virtual device in various ways and various states in the Android Studio project
tags: [Kotlin, Android, UI, Android Studio]
comments: true
---

## Method 1:  Select configure from Project Selection screen
1. Open Android Studio
2. In the bottom right corner, there is a link that says `configure`
![Project Select box](/assets/img/android-studio-project-selection.png)
3. Once in the configure menu, select `AVD Manager`
![AVD Manager](/assets/img/android-studio-project-selection-configure.png)

## Method 2: Tools -> AVD Manager
1. Open Android Studio
2. Open or create a project
3. In the menu bar, select `Tools -> AVD Manager`


## Bonus - Method 3: Select a device when no device is represent
If you are in a project and have no physical devices connected and no virtual devices created.
1. In the top bar, right below the menu bar, you'll see a dropdown that says `No devices`
![Actions Bar](/assets/img/no-devices-menu.png)
2. Select the `No Devices` dropdown and Select `AVD Manager`
![AVD Manager](/assets/img/no-devices-dropdown.png)


## Creating an AVD
![AVD Manager](/assets/img/avd-manager.png)

If you've made it this far, great, you're only a couple more clicks away from having a debuggable testing device.

1. Select `Create Virtual Device`
2. Any device will work on this screen, but if you have plans to include [Google Play Services](https://developers.google.com/android/guides/overview) in your app, I suggest you select a device with Google Play Services installed. You'll see an icon under `Play Store` if this is the case. Select `Next`
3. Download/Select the most recent System Image or the one most applicable to your Project. Select `Next`
4. Select `Finish` on the next screen.
5. You have an AVD! Now just select the play button all the way to the right and you're ready to go!

Congratulations.
