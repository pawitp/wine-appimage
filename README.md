# Wine AppImage
This repository contains code and patches to build 32-bit [Wine](https://winehq.org)
with included 32-bit libraries so it can be ran on 64-bit systems.

## Usage
Run `./wine` and the desired Windows `.exe` file to run.

## Building
This repository is built using GitHub Actions.

## Applied patches
 - wineldpreload.patch - use 32-bit loader to run Wine, required for usage on 64-bit
   systems without 32-bit libraries
   ([credit](https://github.com/Hackerl/Wine_Appimage/issues/11#issuecomment-445724165))
 - line-hack.patch - hack to not create border in LINE app which remains on top even
   when the LINE main window is covered by other apps
   ([credit](https://bugs.winehq.org/show_bug.cgi?id=34631))
