# Alpine Linux with JWM
Mini JWM desktop image with firefox and minimal utilities.

***Note**: Audio support is not included.*

## Install packages

<pre>$ sudo apk add jwm xorg-server udev xinit dbus-x11 libdrm libinput neofetch zip unzip tar conky lxdm xarchiver evince consolekit2 motif feh lxterminal baobab galculator gnome-screenshot arandr firefox network-manager-applet wget python3 pcmanfm leafpad</pre>

## Create JWM session

<pre>
cat > /usr/share/xsessions/jwm.desktop << "EOF"
[Desktop Entry]
Encoding=UTF-8
Name=JWM
Comment=This is the JWM window manager
Exec=/usr/bin/jwm
Type=Application
EOF
</pre>

Alpine Linux JWM Utilities

- **conkyrc**: Place in $HOME folder. Then, rename it to .conkyrc
- **system.jwmrc**: Place in $HOME folder. Then, rename it to .jwmrc
- **background-image.jpg**: Place in $HOME folder.
- **Copy remaining folders**: `$ sudo cp -r etc/ / && sudo cp -r usr/ /`
