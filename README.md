# STZTaskPulse

Minimal Rainmeter skin to show CPU, RAM, and GPU usage in a single line, made to sit above the taskbar. Optional Disk and Network meters can be toggled via a small settings UI.

## Features
- CPU, RAM, GPU usage in one line
- Optional Disk activity and Network down/up
- Always on top (can be changed)
- Lightweight and clean layout

## Requirements
- Windows + Rainmeter (4.3+ recommended for UsageMonitor)

## Install
1) Copy this folder to `Documents\Rainmeter\Skins\STZTaskPulse`
2) In Rainmeter: refresh and load `STZTaskPulse.ini`
3) (Optional) Load `Settings\Settings.ini` to toggle Disk/Net

## Settings UI
The settings panel writes to `STZTaskPulseSettings.inc` and refreshes the main skin.

Toggle options:
- Disk usage
- Network down/up

## Customize
Edit `STZTaskPulse.ini`:
- `FontName`, `FontSize`, `FontColor`
- `BlockW`, `Gap`, `NetBlockW`
- `ZPos=2` keeps the skin always on top

Edit `STZTaskPulseSettings.inc`:
- `ShowDisk=1` or `0`
- `ShowNet=1` or `0`
- `NetInterface=Best` (or a specific interface)
- `DiskInstance=_Total`
- `GPUInstance=_Total`

## GPU / Disk troubleshooting
If GPU or Disk shows text like "Total" or stays at 0:
1) Set `GPUList=1` in `STZTaskPulseSettings.inc`
2) Refresh the skin and check the Rainmeter log for available instances
3) Set `GPUInstance=...` (or `DiskInstance=...`) to a valid entry
4) Set `GPUList=0` again

## File layout
```
STZTaskPulse.ini
STZTaskPulseSettings.inc
Settings/Settings.ini
```

## Notes
- Always-on-top skins will sit above most windows; you can change `ZPos` if needed.


## ⚖️ Licensing (Dual Licensing)

STZTaskPulse is available under two distinct licenses:

1) Community Use (GPLv3): Free for personal use and open-source projects. You are free to modify and distribute this skin, provided that your changes remain open-source.

2) Commercial Use: For companies wishing to integrate this system monitor or its toggle logic into proprietary software, OEM desktop themes, or commercial kiosk interfaces.

To acquire a commercial license, please contact: [starzynhobr@gmail.com]