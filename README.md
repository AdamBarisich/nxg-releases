# NXG Takeoff — releases

Downloads and the version file for **NXG Takeoff**, the plan takeoff and
estimating app used by NeXGen Custom Builders.

**The application source is not in this repository.** This holds only the built
downloads and one small file the app reads to know whether a newer build exists.

## Installing for the first time

Take the `.pkg` from the [latest release](../../releases/latest).

The app is not signed by Apple, so the first time you open the installer macOS
will say it is from an unidentified developer. Right-click the `.pkg` and choose
**Open**, then **Open** again. After that it installs normally.

## Updating

You do not need this page. An installed copy checks for itself, downloads the
new build in the background, and installs it when you quit.

## latest.json

What an installed copy reads. It carries the build number, the download
addresses, a SHA-256 for each file, and a signature.

The signature is the part that matters. The app ships the public half of a key
whose private half exists on one machine and is never uploaded. A version file
that is not signed with that key is refused — so getting write access to this
repository is not enough to push an update to anyone.
