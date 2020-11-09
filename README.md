<h1 align="center">Budgie Clipboard Manager</h1>
A clipboard manager applet that can help you to store and manage clipboard content on the Budgie desktop, Written using Vala.

# Dependencies for Building from source

### *For Solus* 

- `sudo eopkg it budgie-desktop-devel accountsservice-devel alsa-lib-devel gnome-bluetooth-devel gtk-doc gnome-settings-daemon-devel ibus-devel libgnome-desktop-devel libgnome-menus-devel libnotify-devel libpeas-devel libwnck-devel mutter-devel pulseaudio-devel sassc upower-devel vala -c system.devel`

### *For Debian/ Ubuntu or its Derivatives* 

- `sudo apt install budgie-core-dev libglib2.0-dev libgtk-3-dev libpeas-dev meson valac`

### *For Arch or its Derivatives*
- `sudo pacman -S budgie-desktop json-glib libgee libpeas intltool meson ninja vala`

# Building from source
Run from the repo's folder:

- `mkdir build && cd build`

- `meson --buildtype plain --prefix=/usr --libdir=/usr/lib`

- `ninja`

- `sudo ninja install`

