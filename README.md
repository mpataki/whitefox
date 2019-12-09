
### Installation:
- Install the dfu utility with `brew install dfu-util` on macos, or `pacman -S dfu-util` on arch.
- Install the firmware with `dfu-util -D kiibohd.dfu.bin`.

To change the layout, follow the instructions here: [whitefox configurator](https://input.club/configurator-whitefox/). If these don't exist anymore for some reason, try this on arch:

```
pacman -S dfu-util
sudo cp 98-kiibohd.rules /etc/udev/rules.d
sudo udevadm control --reload-rules
sudo udevadm trigger
./kiibohd-configurator-1.0.2-linux-x86_64.AppImage
```

This should start a GUI from the input club folk.
