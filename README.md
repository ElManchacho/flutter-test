# flutter-test

## Install Flutter

#### 1 - Create a the `src` folder at the root of you disk (with path like `C:\src\`) and open a powershell terminal in it

#### 2 - Run `git clone https://github.com/flutter/flutter.git -b stable`

I had an issue with the computer of my company (probably due to security rules) and the clone command were never ending.

#### 2(bis) - If the last cloning command didn't work properly, extract SDK folder in the `src` folder :

You can always download and extract the folder after downloading it here : https://docs.flutter.dev/get-started/install/windows

Version installed for this test was downloaded here : https://storage.googleapis.com/flutter_infra_release/releases/stable/windows/flutter_windows_3.3.5-stable.zip

#### 3 - Add your newly imported flutter `bin` subfolder repository to your system environnement variables

#### 4 - Restart your VSCode and/or console/terminal (powershell, cmd, etc...)

#### 5 - Run `where.exe flutter dart` to check if the environnement variable is well established

#### 6 - Run `flutter doctor` (or `flutter doctor --android-licenses` if the cmdlet advise you to and accept all licenses) in the `src` folder to check if all the software dependencies are installed


```bash
It will look like this : 

PS C:\windows\system32> flutter doctor
Doctor summary (to see all details, run flutter doctor -v):
[√] Flutter (Channel stable, 3.3.5, on Microsoft Windows [version 10.0.19042.2130], locale fr-FR)
[!] Android toolchain - develop for Android devices (Android SDK version 33.0.0)
    X cmdline-tools component is missing
      Run `path/to/sdkmanager --install "cmdline-tools;latest"`
      See https://developer.android.com/studio/command-line for more details.
    X Android license status unknown.
      Run `flutter doctor --android-licenses` to accept the SDK licenses.
      See https://flutter.dev/docs/get-started/install/windows#android-setup for more details.
[√] Chrome - develop for the web
[!] Visual Studio - develop for Windows (Visual Studio Community 2022 17.3.6)
    X Visual Studio is missing necessary components. Please re-run the Visual Studio installer for the "Desktop
      development with C++" workload, and include these components:
        MSVC v142 - VS 2019 C++ x64/x86 build tools
         - If there are multiple build tool versions available, install the latest
        C++ CMake tools for Windows
        Windows 10 SDK
[√] Android Studio (version 2021.3)
[√] VS Code (version 1.72.2)
[√] Connected device (3 available)
[√] HTTP Host Availability

! Doctor found issues in 2 categories.
```

If you found the 'cmdline-tools' error, follow this tutorial : https://www.fluttercampus.com/guide/202/cmdline-tools-component-is-missing-error-flutter/

# Ressources

## Documentation

Installation : https://docs.flutter.dev/get-started/install

