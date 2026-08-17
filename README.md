# 🌟 Solunar

<p align="center">
  <img src="preview/WingsofSilence_Prv.png" alt="Solunar Wings of Silence Theme Preview" width="800px" style="border-radius: 8px; box-shadow: 0 4px 20px rgba(0, 0, 0, 0.35);" />
</p>

<p align="center">
  <a href="https://github.com/Frozen-47/Solunar/stargazers"><img src="https://img.shields.io/github/stars/Frozen-47/Solunar?style=for-the-badge&color=8A2BE2" alt="GitHub stars"></a>
  <a href="https://github.com/Frozen-47/Solunar/blob/main/LICENSE"><img src="https://img.shields.io/github/license/Frozen-47/Solunar?style=for-the-badge&color=blue" alt="License"></a>
  <img src="https://img.shields.io/badge/Vencord-Compatible-success?style=for-the-badge&logo=discord&logoColor=white&color=5865F2" alt="Vencord Compatible">
  <img src="https://img.shields.io/badge/Platform-Windows%20%7C%20macOS%20%7C%20Linux-darkgreen?style=for-the-badge" alt="Platforms">
</p>

---

**Solunar** is a premium, highly customizable, modern CSS theme framework for Discord client modifications (like **Vencord** and **Vesktop**). Built with high-performance glassmorphism, responsive variables, and elegant animations, Solunar transforms your Discord UI into a sleek, clean, and distraction-free workspace.

This repository features the core Solunar base styles alongside two pre-configured, stunning presets:
* 🪶 **Wings of Silence**: A clean, minimalist dark-slate theme with soft layouts.
* 📓 **Death Note (L)**: A monochromatic black-and-white theme featuring gothic crimson accents and old-script typography inspired by the investigator L.

---

## ✨ Features

* **🎭 True Glassmorphism:** Features high-performance frosted-glass blur effects (`backdrop-filter`) across sidebars, popouts, and user profile modals.
* **🌓 Adaptive Shading:** Comes with native variables designed to adapt perfectly to all of Discord's default themes:
  * *Midnight* (deep, ultra-dark overlays)
  * *Darker* (high-contrast dark mode)
  * *Dark* (standard sleek dark styling)
  * *Light* (clean and soft light-glass aesthetics)
* **🎨 Complete Customization:** Tweak colors, fonts, wallpapers, margins, and layout behavior easily by editing a few CSS variables in your `:root`.
* **🖌️ Custom Scrollbars:** Sleek, minimalist, color-matched scrollbars that blend smoothly into the interface.
* **💬 Redefined Chat UI:** Replaces boxy inputs and borders with elegant floating panels, custom reactions, and clean separators.
* **📢 Gorgeous Voice Interface:** The customized voice channel grid and status badges display elegantly with custom glow effects.

---

## 📸 The Themes

### 1. Wings of Silence
A minimalist, high-tech workspace styled with sleek grey and white tones, soft glass blurs, and clean font rendering.
* **Background Image:** [WingsofSilence.png](images/WingsofSilence.png)
* **Custom Theme File:** [WingsofSilence.css](vencord_themes/WingsofSilence.css)

### 2. Death Note (L)
A highly stylized tribute to the legendary detective L. It features a fully desaturated background, blood-crimson indicators, serif typography (`IM Fell English`), custom search inputs, and L's signature glyph as the home icon.
* **Background Image:** [L.png](images/L.png)
* **Custom Theme File:** [DeathNote.css](vencord_themes/DeathNote.css)

---

## 🚀 Installation Guide

### Vencord / Vesktop (Recommended)

You can load these themes dynamically into Vencord by importing the raw GitHub CDN links. This ensures your theme stays up-to-date automatically whenever the base files are updated.

#### Method 1: Quick Online Import (Recommended)
1. Open Discord and go to **User Settings** -> **Themes**.
2. Under **Online Themes**, paste one of the following URLs:
   * **Wings of Silence:**
     ```link
     https://cdn.jsdelivr.net/gh/Frozen-47/solunar@main/vencord_themes/WingsofSilence.css
     ```
   * **Death Note (L):**
     ```link
     https://cdn.jsdelivr.net/gh/Frozen-47/solunar@main/vencord_themes/DeathNote.css
     ```
3. Click **Add Theme** or press Enter. The theme will load instantly!

#### Method 2: Custom CSS (Direct Paste)
If you'd rather copy the code directly:
1. Open Discord and navigate to **User Settings** -> **Custom CSS** (under Vencord).
2. Copy the full CSS code from either [WingsofSilence.css](vencord_themes/WingsofSilence.css) or [DeathNote.css](vencord_themes/DeathNote.css).
3. Paste it directly into the editor and click **Enable**.

---

## 🛠️ Customization Guide

You can easily customize either theme by overriding the default CSS variables. Simply wrap your changes in a `:root` block at the bottom of your Custom CSS editor.

Here is a list of the primary variables you can adjust:

| CSS Variable | Description | Example Value |
|:---|:---|:---|
| `--main-color` | The accent color of the theme (badges, unread dots, active buttons). | `#c0392b` *(Crimson)* |
| `--hover-color` | The hover state of accent elements. | `#922b21` *(Deep Crimson)* |
| `--background-image` | The URL of your main background wallpaper. | `url('https://example.com/wallpaper.jpg')` |
| `--background-filter` | Filters applied to the background image (blur, brightness, saturation). | `saturate(0) brightness(0.35)` |
| `--background-shading-percent` | Controls the opacity layer of your theme shading. | `100%` / `80%` |
| `--main-font` | The primary font family used throughout the app. | `"IM Fell English", serif` |
| `--code-font` | The font used in code block formatting. | `"Courier New", monospace` |
| `--border-color` | Border lines styling (separators, margins). | `rgba(255, 255, 255, 0.07)` |

### Customization Example:
```css
/* Customizing the Death Note theme accent colors & font */
:root {
  --main-color: #3498db;         /* Change blood red to bright blue */
  --hover-color: #2980b9;        /* Hover color to darker blue */
  --main-font: "Outfit", sans-serif; /* Modern sans-serif typography */
  --background-filter: saturate(1) brightness(0.5) blur(4px); /* Add blur, restore color */
}
```

---

## 📂 Repository Structure

```files
├── images/
│   ├── L.png                 # Death Note background asset
│   └── WingsofSilence.png    # Wings of Silence background asset
├── preview/
│   └── WingsofSilence_Prv.png # Main visual preview of the layout
├── theme/
│   ├── main.css              # Core structural style overrides for Discord
│   └── vencord.css           # Vencord-specific elements (plugins, settings, etc.)
└── vencord_themes/
    ├── DeathNote.css         # Theme preset: L (Death Note)
    └── WingsofSilence.css    # Theme preset: Wings of Silence 
```

---

## 🤝 Contributing & Support

If you run into any layout issues, broken selectors (due to Discord client updates), or want to suggest new customizations:
1. Check the [Issues](https://github.com/Frozen-47/Solunar/issues) page to see if someone has already reported the bug.
2. Submit a Pull Request if you'd like to update selectors or add features to the core theme files.

---

### 📜 License
This project is licensed under the [MIT License](LICENSE). Feel free to modify and share your own custom presets!
