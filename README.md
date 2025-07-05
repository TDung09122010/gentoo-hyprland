<div align="center">

# 【 end_4's Hyprland Dotfiles for Fedora 】

 Automated setup of the Quickshell version of end_4's dotfiles on **Fedora Linux**  


</div>

---

## ⚠️ Fedora Workstation Only

This script is intended for **Fedora Workstation** and only **x64 Systems**, other non-atomic variants like KDE Plasma should also work, but they have not been tested.
For the Arch version, visit: [end-4/dots-hyprland](https://github.com/end-4/dots-hyprland)

> ✅ **Tested on Fedora 42**

---


<div align="center">
    <h2>• screenshots •</h2>
    <h3></h3>
</div>

## illogical-impulse<sup>Quickshell</sup>

| AI | Common widgets |
|:---|:---------------|
| ![image](https://github.com/user-attachments/assets/08d26785-b54d-4ad1-875b-bb08cc6757f5) | ![image](https://github.com/user-attachments/assets/4fcd63d9-0943-4b21-8737-4bed97b71961) |
| Window management | Weeb power (sigh)|
| ![image](https://github.com/user-attachments/assets/86cc511b-0d33-4c78-bcc0-3037d02a17da) | ![image](https://github.com/user-attachments/assets/292259fc-57d3-4663-a583-2ce2faad13fb) |

By the way...
- The funny notification positions are mimicking Android 16's dragging behavior
- The clock on the wallpaper is automatically placed at the "least busy" region of the image

## Installation

### First read the notes section, this is not optional.

Run the automatic installer:

```bash
bash <(curl -s https://raw.githubusercontent.com/EisregenHaha/fedora-hyprland/f42/setup.sh)
```
or if you are using fish shell (non-posix-compliant shell) then:
   
```bash
bash -c "$(curl -s https://raw.githubusercontent.com/EisregenHaha/fedora-hyprland/f42/setup.sh)"
```

Then **reboot** and select the **Hyprland (non-uwsm)** session to log in.

---

## Updating

To update the configs:

1. Make sure you have read the Notes
2. Run the script again.
3. Select **option 1** again in the menu.

---

## Notes

### Configurations
- Custom configurations like enabling/disabling the dock or similar happen in `.config/illogical-impulse/config.json`.
- To change your Icon pack you will need to select it in KDE Settings and then also change the configuration in  `.config/kde-material-you-colors/config.conf`

### Regarding Updates
- Place any custom Hyprland config changes in `.config/hypr/custom` and then comment out the old configuration in `.config/hypr/hyprland.conf`.
- These files are **not overwritten** by the update process. Otherwise you **will** lose your configuration changes after updating.  
  
### For Nvidia users:
- Uncomment the lines found in `~/.config/hypr/custom/env.conf`

### Common fixes
- The Dark/Light and theme switcher wont work on first login, please select the "6) Update config files with exclusions" in the setup after your initial login to fix the permission error.
- If you want to raise your volume above the limit of 90, open `~/.config/illogical-impulse/config.json` and set the max volume allowed to 100. This is just a safety measure.
- If you're experiencing missing or broken icons, try switching your icon pack in the KDE settings, it's an issue with Adwaita. I use the Colloid icon pack.

### Keybinds
  
   - **Default keybinds**: Should be somewhat familiar if you've used Windows or GNOME. 
     - For a list, hit `Super`+`/`
     - For a terminal, hit `Super`+`Enter`


### Archive (not needed)
- Original (outdated) discussion: [#840](https://github.com/end-4/dots-hyprland/discussions/840)
---

## Thanks

- [@Kamion008](https://github.com/Kamion008) – Fedora version  
- [@nullptroma](https://github.com/nullptroma) – Original OpenSUSE script Kamion008 used

                        
## stars because i like big numbers
[![Stargazers over time](https://starchart.cc/EisregenHaha/fedora-hyprland.svg?variant=adaptive)](https://starchart.cc/EisregenHaha/fedora-hyprland)

                    
