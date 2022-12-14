---
uid: installation-macos
title: MacOS
description: Install on MacOS.
sidebar_position: 5
---

<!-- markdownlint-disable MD036 no-emphasis-as-heading -->

# Install on MacOS

macOS Application packages and builds in TAR archive format are available [here](/downloads/macos).

**Install**

1. Download the latest version.
2. Drag the `.app` package into the Applications folder.
3. Start the application.
4. Click the icon in the menu bar and select "Launch Web UI".

**Upgrade**

1. Download the latest version.
2. Stop the currently running server either via the dashboard or using the menu bar icon.
3. Drag the new `.app` package into the Applications folder and click yes to replace the files.
4. Start the application.

**Uninstall**

1. Stop the currently running server either via the dashboard or using the application icon.
2. Move the `.app` package to the trash.

**Deleting Configuration**

This will delete all settings and user information. This applies for the .app package and the portable version.

1. Delete the folder `~/.config/jellyfin/`
2. Delete the folder `~/.local/share/jellyfin/`

**Portable Version**

1. Download the latest version
2. Extract it into the Applications folder
3. Open Terminal and type `cd` followed with a space then drag the jellyfin folder into the terminal.
4. Type `./jellyfin` to run jellyfin.
5. Open your browser at <http://localhost:8096>

Closing the terminal window will end Jellyfin. Running Jellyfin in screen or tmux can prevent this from happening.

**Upgrading the Portable Version**

1. Download the latest version.
1. Stop the currently running server either via the dashboard or using `CTRL+C` in the terminal window.
1. Extract the latest version into Applications
1. Open Terminal and type `cd` followed with a space then drag the jellyfin folder into the terminal.
1. Type `./jellyfin` to run jellyfin.
1. Open your browser at <http://localhost:8096>

**Uninstalling the Portable Version**

1. Stop the currently running server either via the dashboard or using `CTRL+C` in the terminal window.
1. Move `/Application/jellyfin-version` folder to the Trash. Replace version with the actual version number you are trying to delete.

**Using FFmpeg with the Portable Version**

The portable version doesn't come with FFmpeg by default, so to install FFmpeg you have three options.

- use the package manager homebrew by typing `brew install ffmpeg` into your Terminal ([here's how to install homebrew if you don't have it already](https://treehouse.github.io/installation-guides/mac/homebrew)
- download the most recent static build from [this link](https://evermeet.cx/ffmpeg/get/zip) (compiled by a third party see [this page](https://evermeet.cx/ffmpeg/) for options and information), or
- compile from source available from the official [website](https://ffmpeg.org/download.html)

More detailed download options, documentation, and signatures can be found.

If using static build, extract it to the `/Applications/` folder.

Navigate to the Playback tab in the Dashboard and set the path to FFmpeg under FFmpeg Path.
