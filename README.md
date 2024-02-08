# difhel's rising on MX Linux 23 (XFCE)
## Where do we start?
- OS: MX Linux 23 Libretto (based on Debian 12 Bookworm) - midweight stable Linux distro
- Desktop environment (DE): XFCE4
- Compositor: moved from default xfwm4 to [picom](https://github.com/yshui/picom), fork of [compton](https://github.com/chjj/compton) - a lightweight and powerful compositor for X11
## What's shipped in?
- window rounded corners
- background blur for XFCE Terminal and all applications that uses RGBA background
- beautiful window switcher (Alt + Tab)
- CSS-modified [Orchis Purple Dark](https://github.com/vinceliuice/Orchis-theme) theme
- Mac OS styled window buttons
- some windows animations
- very beautiful `xfce4-panel` with plugins (action buttons, Verve command line, docklike taskbar, clock & date, Pulseaudio, status tray, launcher), customized with some GTK CSS

## How to use
### GTK Theme
Copy `Orchis-Purple-Dark` to yours `/usr/share/themes`, then select this theme in XFCE settings application.

### XFCE Panel
1. Copy the GTK theme, because all of CSS modifications were inserted in `Orchis-Purple-Dark/gtk-3.0/gtk.css`
2. Install this plugins and panel settings:

    <img src="https://github.com/difhel/xfce-dotfiles/assets/78644136/8535a0b9-cb8a-4733-bba8-4b7f8a725b0f" width="300px"/>
    <img src="https://github.com/difhel/xfce-dotfiles/assets/78644136/1782d0b5-d7f4-4b1a-87cc-04a7f77b14bb" width="300px"/>
    <img src="https://github.com/difhel/xfce-dotfiles/assets/78644136/aa2f2b06-6f47-48d2-b234-7c14c9cc64f3" width="300px"/>

### Compositor
1. Install [picom](https://github.com/yshui/picom)
2. Copy `compton.conf` to `~/.config/compton.conf`

## How to debug
You can use GTK Inspector for some system apps like `xfce4-panel`
```shell
GTK_DEBUG=interactive xfce4-panel
```

## What does it look like?
https://www.reddit.com/r/unixporn/comments/17ocwta/xfce_my_first_xfce_rising/

![image](https://github.com/difhel/xfce-dotfiles/assets/78644136/69463bb4-560b-4b34-a4b0-1bb8e13b58d3)

![image](https://github.com/difhel/xfce-dotfiles/assets/78644136/bae12d46-b4ce-4fb1-92f4-032b62fda3e5)

![image](https://github.com/difhel/xfce-dotfiles/assets/78644136/4560ecbc-66da-4cea-899d-d6e2d556c49b)

## Issues
If you encounter any issues, I urge you to try to figure it out yourself and submit a pull-request rather than creating an issue. This repository is the result of my experiment with XFCE. I don't use it all the time, I don't have access to a configured version of it, I'm unlikely to be able to help you fix any bug. But I'm always happy to improve my dotfiles and publish it publicly, so I look forward to your pull-requests!
