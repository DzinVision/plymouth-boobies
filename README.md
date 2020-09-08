# Plymouth Boobies
Boobies theme for plymouth based on [this GIF](https://icon-library.net/icon/loading-icon-animated-gif-2.html).

![gif](https://icon-library.net//images/loading-icon-animated-gif/loading-icon-animated-gif-2.jpg)

## Installing
- archlinux:
```bash
# add theme to plymouth dir
sudo mkdir /usr/share/plymouth/themes/boobies
sudo cp -r . /usr/share/plymouth/themes/boobies

# check that theme exists
sudo plymouth-set-default-theme -l

# set theme as default
sudo plymouth-set-default-theme -R boobies
```
- debian based distros:
```bash
# add theme to plymouth dir
sudo mkdir /usr/share/plymouth/themes/boobies
sudo cp -r . /usr/share/plymouth/themes/boobies

# install theme
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/boobies/boobies.plymouth 100

# apply the theme (select the number of installed theme)
sudo update-alternatives --config default.plymouth

# update initramfs
sudo update-initramfs -u
```

## Credits
Template for plymouth config is written by [adi1090x](https://github.com/adi1090x). He has a [big collection](https://github.com/adi1090x/plymouth-themes/) of plymouth themes that you should check out.