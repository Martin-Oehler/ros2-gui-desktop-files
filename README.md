# ros2-gui-desktop-files

This repository contains GNOME .desktop files for common ros2 GUI tools.

For some reason, newer versions of Ubuntu, e.g. 24.04, require a desktop file to display an icon in the left application pane. Such a file is not automatically installed, making Ubuntu default to a grey question mark. This repository provides the necessary desktop files to restore the icon.

## Installation

First, clone this repository and go inside the folder:

```
git clone https://github.com/Martin-Oehler/ros2-gui-desktop-files.git
cd ros2-gui-desktop-files
```

Now copy over the files:

```
cp *.desktop ~/.local/share/applications
```

## Notes

- It should be possible for packages to install their desktop files automatically, but I did not investigate this further
- The paths are hard-coded for ros2 jazzy. The entries can likely be improved by using the `ROS_DISTRO` environment variable instead.
- Gazebo does not include their icon, therefore, it has to be manually copied to an indexed icon folder
