# Xorg
path: /etc/X11/xorg.conf.d/

## 00-keyboard.conf
```
Section "InputClass"
        Identifier "system-keyboard"
        MatchIsKeyboard "on"
        Option "XkbLayout" "us"
        Option "XkbModel" "pc105+inet"
        Option "XkbOptions" "caps:swapescape"
EndSection
```

## 20-intel.conf
```
Section "Device"
	Identifier  "Intel Graphics"
	Driver      "intel"
	Option      "DRI" "iris"
EndSection
```

## 30-touchpad.conf
```
Section "InputClass"
    Identifier "touchpad"
    Driver "libinput"
    MatchIsTouchpad "on"
    Option "Tapping" "on"
    Option "TappingButtonMap" "lmr"
    Option "NaturalScrolling" "true"
EndSection
```
