<p align="center"><a href="#budgie-clipboard-manager"><img src="https://raw.githubusercontent.com/prateekmedia/budgie-clipboard-applet/main/images/clipmgr.png" height=80px alt="Clipboard manager Logo"/></a></p>
<h1 align="center">Budgie Clipboard Manager</h1>
<p align="center">
<a href="https://github.com/prateekmedia/budgie-clipboard-applet/releases"><img alt="GitHub release" src="https://img.shields.io/github/v/release/prateekmedia/budgie-clipboard-applet"/></a> <a href="LICENSE"><img alt="License" src="https://img.shields.io/github/license/prateekmedia/budgie-clipboard-applet?color=blue"/></a>
</p>

A clipboard manager applet that can help you to store and manage clipboard content. 
***Made with ♥️ for budgie desktop.***

<p align="center"><img src="https://raw.githubusercontent.com/prateekmedia/budgie-clipboard-applet/main/images/screenshot.png" alt="Screenshot"/></p>

## FEATURES
- [x] Clipboard history management
- [x] Save up to 100 Clips
- [x] Private mode 
- [x] Remove any clip you  want
- [x] Searchable history
- [x] Clear all option
- [x] Autosave History
- [x] Notification support
- [x] Customizable Applet
- [x] Restore Defaults Option
- [x] Automatically paste selected clip to active window

## CONTRIBUTION
-  Pull requests are welcome whether it be [translations](https://github.com/prateekmedia/budgie-clipboard-applet/releases/tag/v0.9.8), adding any useful feature / solving any bugs
-  You can use `Issues` tab for reporting issues
-  Special thanks to [all these amazing people](https://github.com/prateekmedia/budgie-clipboard-applet/graphs/contributors) who contributed to this project.

## Direct Install
**For Debian/ Ubuntu based Distro**
```
$ sudo add-apt-repository ppa:ubuntubudgie/backports

$ sudo apt install budgie-clipboard-applet
```


## Dependencies for Building from source
These dependencies are required if you want to [Build From Source](#Building-from-source)

**For Solus**
```
$ sudo eopkg it budgie-desktop-devel vala -c system.devel xdotool
```

**For Debian/ Ubuntu based Distro**
```
$ sudo apt install budgie-core-dev meson valac xdotool
```
**For Arch based Distro**
```
$ sudo pacman -S budgie-desktop xdotool
```
**NOTE** : `xdotool` is optional and is used for pasting text in active window.

## Building from source
Download the [zip](https://github.com/prateekmedia/budgie-clipboard-applet/archive/main.zip) & then run from the extracted repo's folder:

```
$ mkdir build

$ meson --buildtype plain build --prefix=/usr --libdir=/usr/lib

$ sudo ninja -C build install
```
**NOTE** : *You can also update the applet by following the above 3 step process*

## For reinstalling / Uninstalling
If you want to reinstall the applet, then run this from the extracted repo's folder:

```
$ sudo ninja -C build install
```
Likewise the applet can be **uninstalled** by using 
```
$ sudo ninja -C build uninstall
```

### Debug the applet
```
$ budgie-panel --replace &!
```
