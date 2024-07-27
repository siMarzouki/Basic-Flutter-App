# First application

Now, we will create our first flutter app and test everything.

[![YouTube video player](https://img.youtube.com/vi/mmtuEKcvY3g/0.jpg)](https://www.youtube.com/embed/mmtuEKcvY3g)

1. Run **flutter doctor** to check again that all dependencies are completed.
2. Invoke View > Command Palette. (Ctrl + Shift + P)
3. Type “flutter”, and select the Flutter: New Application Project.
4. Create or select the parent directory for the new project folder.
5. Enter a project name, such as **first_app**, and press Enter.
6. Wait for project creation to complete and the main.dart file to appear.
7. Run **flutter emulators** to check the available emulators.
8. Invoke **Run > Run Without Debugging** (Ctrl + F5).
9. Wait for the app to launch.
10. Change the **primarySwatch** from **Colors.blue** to **Colors.green**.
11. Save your changes: invoke Save All (Ctrl + S), or click Hot Reload to see the updated color in the running app almost immediately.

![Hot Reload & Hot Restart in Flutter](https://firebasestorage.googleapis.com/v0/b/flutter-pro-51469.appspot.com/o/c1l5p1.png?alt=media&token=136ef0f0-2445-4dac-9be8-5871abe8bc9e)

### What is the difference between hot reload, hot restart, and full restart?

**Hot reload** loads code changes into the VM and re-builds the widget tree, preserving the app state; it doesn’t rerun main() or initState(). (F5 in VSCode)

**Hot restart** loads code changes into the VM, and restarts the Flutter app, losing the app state. (⇧ F5 in VSCode)

**Full restart** restarts the iOS, Android, or web app. This takes longer because it also recompiles the Java / Kotlin / ObjC / Swift code. On the web, it also restarts the Dart Development Compiler. There is no specific keyboard shortcut for this; you need to stop and start the run configuration.

Flutter web currently supports hot restart but not hot reload.
