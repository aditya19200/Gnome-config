# 🌟 Elegant GNOME Desktop Configuration

## 📦 Prerequisites
- GNOME 40+
- dconf
- gnome-tweaks
- gtk-engine-murrine
- papirus-icon-theme

## 🎨 Theming

### Install Recommended Themes
```bash
# Install User themes and icon themes
sudo apt install gnome-shell-extensions gnome-tweaks papirus-icon-theme
```

### Gnome Shell Configuration
```bash
# Disable desktop icons
gsettings set org.gnome.shell.extensions.desktop-icons show-home false
gsettings set org.gnome.shell.extensions.desktop-icons show-trash false

# Customize top bar
gsettings set org.gnome.desktop.interface show-battery-percentage true
gsettings set org.gnome.desktop.interface clock-show-seconds true
gsettings set org.gnome.desktop.interface clock-show-weekday true
```

### Appearance Settings
```bash
# Set elegant dark theme
gsettings set org.gnome.desktop.interface gtk-theme 'Adwaita-dark'
gsettings set org.gnome.desktop.interface icon-theme 'Papirus-Dark'
gsettings set org.gnome.desktop.wm.preferences theme 'Adwaita-dark'
```

## 🖥️ Desktop Experience
```bash
# Minimize/Maximize buttons
gsettings set org.gnome.desktop.wm.preferences button-layout 'close,minimize,maximize:appmenu'

# Touchpad and Mouse Settings
gsettings set org.gnome.desktop.peripherals.touchpad tap-to-click true
gsettings set org.gnome.desktop.peripherals.touchpad two-finger-scrolling-enabled true

# Animation and Performance
gsettings set org.gnome.desktop.interface enable-animations true
```

## 🔧 Recommended Extensions
- User Themes
- Dash to Dock
- Blur My Shell
- Caffeine
- Applications Menu

### Install Extensions Script
```bash
#!/bin/bash
EXTENSIONS=(
    "user-theme@gnome-shell-extensions.gcampax.github.com"
    "dash-to-dock@micxgx.gmail.com"
    "blur-my-shell@aunetx"
    "caffeine@eon.uberspace.de"
    "places-menu@gnome-shell-extensions.gcampax.github.com"
)

for ext in "${EXTENSIONS[@]}"; do
    gnome-extensions install "$ext"
done

# Reload GNOME Shell
busctl --user call org.gnome.Shell /org/gnome/Shell org.gnome.Shell Reload
```

## 🌈 Color Scheme
Recommended color palette:
- Background: #121212 (Deep Dark)
- Accent: #3498db (Elegant Blue)
- Text: #ffffff (Clean White)
- Highlight: #2ecc71 (Soft Green)

## 💻 Wallpaper Recommendation
- Minimal, dark-themed wallpapers
- Abstract geometric designs
- Solid color gradients

## 📝 Installation
1. Clone this repository
2. Run configuration scripts
3. Customize to your preference

## 🤝 Contribution
Feel free to fork, star, and contribute!

## 📄 License
MIT License
```

## 🚀 Usage Tips
- Backup your existing configuration before applying
- Customize scripts to match your specific Linux distribution
- Experiment and personalize

## 🔗 Screenshots
<img width="304" alt="image" src="https://github.com/user-attachments/assets/e96b9b80-f952-489d-b869-f058923a9415" />
<img width="310" alt="image" src="https://github.com/user-attachments/assets/4018f9c9-2b58-4d49-8383-967083e47b14" />
<img width="295" alt="image" src="https://github.com/user-attachments/assets/a9cebe15-bb1e-41dd-890b-1635bdae52da" />
