# Tracker PR9 Windows test build

This branch packages the Tracker PR #74 integration against OSP PR #9 as a self-contained Windows x64 application image for testing.

The packaging workflow lives in `.github/workflows/build-windows-pr9.yml`. It overlays the changed OSP and Tracker classes onto the existing Tracker distribution JAR, includes the Windows Xuggle JAR and Tracker assets, and uses `jpackage` to bundle a Java 17 runtime with a native Windows launcher.
