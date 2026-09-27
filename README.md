# morvane-sway-theme

The MorvaneOS look for Sway: the Twilight wallpaper, and MorvaneOS colours for window
borders, titles and Sway's bar. The focused window has a Pastel Pink border as well
as brighter title text, so it isn't told apart by colour alone.

Installs `/etc/sway/config.d/50-morvane-theme.conf`. Sway's default config
(`/etc/sway/config`) ends with `include /etc/sway/config.d/*`, so it applies on top
of Sway's defaults.

**If you make your own `~/.config/sway/config`**, it replaces Sway's default config
and this with it. Add `include /etc/sway/config.d/*` to it to keep the MorvaneOS look.

Terminal (foot) and bar colours come from
[morvane-wm-theme](https://github.com/MorvaneOS/morvane-wm-theme), apps from
[morvane-gtk-theme](https://github.com/MorvaneOS/morvane-gtk-theme). The MorvaneOS
installer installs this package with Sway.

## Changing it

Edit `tools/build.py`, then:

```
python tools/build.py
```

Needs only Python. Commit the output, bump `pkgver`, build and publish.

## License

LGPL-2.1-or-later.
