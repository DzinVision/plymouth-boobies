# Plymouth Boobies
Custom plymouth themes. Includes:
- **boobies** based on [this GIF](https://icon-library.net/icon/loading-icon-animated-gif-2.html).

![gif](boobies/boobies.gif)
- **liquid** based on [this GIF](https://inspiration.design/posts/579294-liquid-preloader).

- **pacman** based on [this GIF](https://inspiration.design/posts/610284-preloader-concept).

![GIF](pacman/pacman.gif)


## Installing
### 1. Plymouth
You need to have plymouth installed and set up - check that it works before proceeding.
### 2. Theme
*Replace `[theme name]` with the desired theme.**
- archlinux:
```bash
sudo cp -r [theme name] /usr/share/plymouth/themes/

# check that theme exists
sudo plymouth-set-default-theme -l

# set theme as default
sudo plymouth-set-default-theme -R [theme name]
```
- debian based distros:
```bash
# add theme to plymouth dir
sudo cp -r [theme name] /usr/share/plymouth/themes/

# install theme
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/[theme name]/[theme name].plymouth 100

# apply the theme (select the number of installed theme)
sudo update-alternatives --config default.plymouth

# update initramfs
sudo update-initramfs -u
```

## Credits
Template for plymouth config is written by [adi1090x](https://github.com/adi1090x). He has a [big collection](https://github.com/adi1090x/plymouth-themes/) of plymouth themes that you should check out.