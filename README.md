# iio-hyprland
Fork of a fork of okeri/iio-sway for Hyprland

**This fork rotates all Tablets and Touch Devices without the need to add them manually.**

Listens to iio-sensor-proxy and automatically changes Hyprland output orientation

## Installing 

:warning: Make sure [iio-sensor-proxy](https://gitlab.freedesktop.org/hadess/iio-sensor-proxy/) running :warning:

### Build from scratch

```
git clone https://github.com/Desktop31/iio-hyprland

cd iio-hyprland

sudo make install
```

## Uninstalling 
```
cd iio-hyprland

sudo make uninstall
```

## Running
`iio-hyprland [monitor to rotate, default=eDP-1]`, run `hyprctl monitors` to list available outputs.

Add `exec-once = iio-hyprland` to `~/.config/hypr/hyprland.conf`

## Touch rotation support

Should automatically rotate all Tablets and Touch Devices from `hyprctl devices`.
