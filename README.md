# Appimage-Updater
Small systemd service with a reasonable footprint. Still pretty basic, but updates an app if the URL stays the same and there is a different file.

It asks the user to enter URLs, so be ready and have your URLs for the apps you want.

Restrictions:
- this script just checks if behind the URL is a new file, if yes it downloads that
- the script currently does not check if the URL is not existent and checks for newer files. This should be possible to implement
  - I think the naming of versions is a mess too. So this could be really difficult to do.
- The script runs daily as a user systemd service. Not all the time, no permissions required.
- It does not handle fancy things like desktop integration.

Install:
```
wget https://github.com/trytomakeyouprivate/Appimage-Updater/raw/main/setup | bash
```
