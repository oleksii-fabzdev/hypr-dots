# hypr-dots

My personal **Arch + Hyprland** desktop configs — the setup from the video.

Built on top of [**JaKooLit's Hyprland-Dots**](https://github.com/JaKooLit/Hyprland-Dots)
(v2.3.20 base) with my own tweaks layered in `hypr/UserConfigs/`. Full credit for the
underlying framework goes to JaKooLit and the wider Hyprland ricing community — this repo
is my customized copy, not original work from scratch.

## What's in here

Everything lives under `.config/`, mirroring `~/.config`:

| Component | Config |
|-----------|--------|
| Compositor | `hypr/` (Hyprland, hyprlock, hypridle) |
| Status bar | `waybar/` |
| App launcher / menus | `rofi/` |
| Terminals | `kitty/`, `ghostty/`, `wezterm/` |
| Notifications | `swaync/` |
| Logout menu | `wlogout/` |
| Shell widgets | `quickshell/`, `ags/` |
| Colors from wallpaper | `wallust/` |
| Audio visualizer | `cava/` |
| System fetch / monitor | `fastfetch/`, `btop/` |
| Screenshot annotate | `swappy/` |
| Qt theming | `Kvantum/`, `qt5ct/`, `qt6ct/` |
| Misc | `mpv/`, `rog/` (Asus ROG) |

My personal changes live mostly in `hypr/UserConfigs/` — keybinds, window rules, startup
apps, environment, animations. That's the JaKooLit-recommended place to customize without
touching the base configs, so it's the first place to look.

## Wallpapers

Not included (they're ~1 GB and mostly the bundled set). Grab them from
[JaKooLit/Wallpaper-Bank](https://github.com/JaKooLit/Wallpaper-Bank) and drop them in
`~/Pictures/wallpapers`.

## Install

The clean path is to install JaKooLit's Hyprland-Dots first, then overlay these files:

1. Run the [Arch-Hyprland installer](https://github.com/JaKooLit/Arch-Hyprland).
2. Back up your existing `~/.config`.
3. Copy this repo's `.config/` over yours:
   ```bash
   git clone https://github.com/<your-username>/hypr-dots
   cp -rb hypr-dots/.config/. ~/.config/
   ```
4. Log out and back into Hyprland.

Things you'll likely want to set for your own machine: `hypr/monitors.conf` (display layout)
and `hypr/UserConfigs/Startup_Apps.conf`.

## Credits

- [JaKooLit — Hyprland-Dots](https://github.com/JaKooLit/Hyprland-Dots) — the base framework
- [ML4W](https://github.com/mylinuxforwork) and theme authors credited inline in the config headers
- The Hyprland project and everyone in the ricing community

---

*On-device configs only — no keys, tokens, or personal data live in this repo.*
