# Install the Google Pixel Camera app, disable GrapheneOS camera app

1. Install [Pixel Camera](https://play.google.com/store/apps/details/?id=com.google.android.GoogleCamera) from the Play Store or [Aurora Store](https://f-droid.org/packages/com.aurora.store/).
2. Check you have enabled the Camera Gesture in **Settings app > System > Gestures > Double press power button** "On: Camera." 
3. Test it at least once by double-pressing the Lock button WHILE THE PHONE IS LOCKED; it may prompt you to unlock the screen to select Google Camera as your default camera app. 
4. You SHOULD only need to do this once, HOWEVER if it keeps prompting you to unlock the screen every time, you can try disabling the GrapheneOS Camera app. (The developers prevent us from disabling this app from the normal App Info interface, so instead...)
5. ...In an ADB shell, execute: `pm uninstall app.grapheneos.camera`.
6. OPTIONAL: If you don't have Google Photos installed (and don't plan to install it), you can install CalyxOS's [GPhotos Preview Stub](https://droidify.app/app/?id=com.google.android.apps.photos&repo_address=https://calyxos.gitlab.io/calyx-fdroid-repo/fdroid/repo) for added functionality.
