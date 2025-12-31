# Zenith Theme for VS Code

**A soothing, aesthetically pleasing colorscheme with soft pastels**

Designed for comfortable long coding sessions with excellent readability

Available in six beautiful variants: **Dusk**, **Dawn**, **Twilight**, **Forest**, **Retro**, and **Ocean**

[Website](https://samonide.github.io/zenith/) • [GitHub](https://github.com/samonide/zenith) • [Report Issue](https://github.com/samonide/zenith-vsc/issues)

---

## ✨ Features

- 🎨 **6 Unique Variants** — From light to dark, warm to cool
- 👁️ **Eye Comfort** — Optimized for long coding sessions  
- 🌈 **Rich Syntax** — Distinct colors for better code reading
- 🎯 **Complete Coverage** — Full VS Code UI theming
- 💜 **Consistent Design** — Same aesthetic across all themes
- 📦 **Regular Updates** — Based on the Zenith color system

---

## 🎨 Variants

### 🌙 **Zenith Dusk** (Default)
The original Zenith experience - a soft pastel dark theme perfect for extended coding sessions. Balanced contrast with soothing colors that won't strain your eyes.

**Background:** `#1e1e2e` • **Accent:** `#bba6f7`

### ☀️ **Zenith Dawn**
A bright and airy light variant for daytime coding. Features gentle pastels on a light background while maintaining the Zenith aesthetic.

**Background:** `#faf7f3` • **Accent:** `#7c3fed`

### 🌃 **Zenith Twilight**
A deeper, moodier dark variant for those late-night coding sessions. Enhanced depth with richer tones and lower brightness.

**Background:** `#0d0d18` • **Accent:** `#9d8dff`

### 🌲 **Zenith Forest**
A calm dark theme with earthy green-gray tones. Perfect for natural, focused coding sessions with reduced eye strain.

**Background:** `#0e1311` • **Accent:** `#98b3d9`

### 🕹️ **Zenith Retro**
A nostalgic warm theme with vintage amber and sepia tones. Inspired by classic CRT terminals and vintage computing aesthetics.

**Background:** `#1a1410` • **Accent:** `#b8b3e8`

### 🌊 **Zenith Ocean**
A serene deep blue theme inspired by calm ocean depths. Cool-toned with vibrant syntax colors for peaceful, focused coding.

**Background:** `#0a0e14` • **Accent:** `#a5b0ff`

---

## 📦 Installation

### From VS Code Marketplace

1. Open **Extensions** sidebar panel in VS Code (`Ctrl+Shift+X` or `Cmd+Shift+X`)
2. Search for **"Zenith Theme"**
3. Click **Install**
4. Click **Reload** to reload your editor
5. Go to `File > Preferences > Theme > Color Theme` and select one of the Zenith variants

### Manual Installation

1. Download the latest `.vsix` file from [Releases](https://github.com/samonide/zenith-vsc/releases)
2. Open VS Code
3. Press `Ctrl+Shift+P` (or `Cmd+Shift+P` on macOS)
4. Type "Install from VSIX" and select the downloaded file

---

## 🚀 Activation

After installation, activate a Zenith variant:

1. Press `Ctrl+K Ctrl+T` (or `Cmd+K Cmd+T` on macOS)
2. Select your preferred variant:
   - **Zenith Dusk** (Default dark)
   - **Zenith Dawn** (Light)
   - **Zenith Twilight** (Deeper dark)
   - **Zenith Forest** (Earthy dark)
   - **Zenith Retro** (Vintage warm)
   - **Zenith Ocean** (Deep blue)

---

## 💡 Recommended Settings

For the best experience with Zenith Theme, add these to your `settings.json`:

```json
{
  "workbench.colorTheme": "Zenith Dusk",
  "editor.fontFamily": "'JetBrains Mono', 'Fira Code', 'Cascadia Code', Menlo, Monaco, 'Courier New', monospace",
  "editor.fontSize": 14,
  "editor.lineHeight": 1.6,
  "editor.fontLigatures": true,
  "editor.cursorBlinking": "smooth",
  "editor.cursorSmoothCaretAnimation": "on",
  "editor.smoothScrolling": true,
  "editor.bracketPairColorization.enabled": true,
  "editor.guides.bracketPairs": true,
  "editor.semanticHighlighting.enabled": true
}
```

### Recommended Font

Zenith looks beautiful with any modern coding font, but we especially recommend:

- [**JetBrains Mono**](https://www.jetbrains.com/lp/mono/) — Clean and readable with ligatures
- [**Fira Code**](https://github.com/tonsky/FiraCode) — Popular choice with excellent ligatures
- [**Cascadia Code**](https://github.com/microsoft/cascadia-code) — Microsoft's modern coding font
- [**MonoLisa**](https://www.monolisa.dev/) — Premium option with excellent readability

---

## 🎯 Language Support

Zenith Theme provides excellent syntax highlighting for:

- **JavaScript/TypeScript** — Full support with semantic highlighting
- **React/JSX** — Beautiful component highlighting
- **Python** — Clear distinction of functions, classes, and decorators
- **Go** — Clean package and function highlighting
- **Rust** — Comprehensive syntax support
- **HTML/CSS** — Elegant tag and property colors
- **JSON/YAML** — Clear structure visualization
- **Markdown** — Beautiful document styling
- **And many more!**

---

## 🔧 Customization

Want to tweak Zenith to your liking? Add custom color overrides in your `settings.json`:

```json
{
  "workbench.colorCustomizations": {
    "[Zenith Dusk]": {
      "editor.background": "#1a1a2a",
      "activityBar.background": "#1a1a2a"
    }
  },
  "editor.tokenColorCustomizations": {
    "[Zenith Dusk]": {
      "comments": "#9090b0"
    }
  }
}
```

---

## 📸 Screenshots

> **Note:** Screenshots coming soon! Check the [website](https://samonide.github.io/zenith/) for live previews.

---

## 🤝 Contributing

Found a bug or have a suggestion? We'd love to hear from you!

1. Check [existing issues](https://github.com/samonide/zenith-vsc/issues)
2. Create a new issue with details
3. Or submit a pull request

---

## 📄 License

MIT License — see [LICENSE](LICENSE) file for details

---

## 🌟 About Zenith

Zenith is a universal colorscheme system designed from the ground up to be:

- **Eye-friendly** — Deep, comfortable backgrounds and soft pastel colors
- **Readable** — High contrast where it matters, subtle where it doesn't
- **Beautiful** — Soothing aesthetic that doesn't distract
- **Universal** — Can be ported to any editor or application

### Other Implementations

- 🎨 [**Main Repository**](https://github.com/samonide/zenith) — Color definitions and website
- 🌙 **Neovim** — Coming soon!
- 🖥️ **Terminals** — Coming soon!

---

<div align="center">

Made with 💜 by [samonide](https://github.com/samonide)

**If you enjoy Zenith, consider giving it a ⭐ on [GitHub](https://github.com/samonide/zenith)!**

</div>
