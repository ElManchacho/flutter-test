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

It will look like this : 

```bash
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

If you find the
```bash
[!] Visual Studio - develop for Windows (Visual Studio Community 2022 17.3.6)
    X Visual Studio is missing necessary components. Please re-run the Visual Studio installer for the "Desktop
      development with C++" workload, and include these components:
        MSVC v142 - VS 2019 C++ x64/x86 build tools
         - If there are multiple build tool versions available, install the latest
        C++ CMake tools for Windows
        Windows 10 SDK
```
error, relaunch the Visual Studio Installer :

![Capture 1](https://user-images.githubusercontent.com/74706889/197215575-7ebc2794-cefb-41ee-b09a-da8c7b535b66.PNG)

Modify the current installation (page corresponding to picture below should appear) :

![Capture 2](https://user-images.githubusercontent.com/74706889/197215682-8ced2c39-b6fc-42a6-8b06-08b9b3e61c6b.PNG)

and click the second section (amon the 4 headers, 'Composants individuels' on the picture, or 'Individual compenents' on an english installation) and search the required module(s), 'MSVC v142 - VS 2019 C++ x64/x86 build tools' in the previous error message :

![Capture](https://user-images.githubusercontent.com/74706889/197216295-1f6253e3-bccc-4a9d-9eb8-3059cdddd027.PNG)



# Ressources

## Documentation

Installation : https://docs.flutter.dev/get-started/install

