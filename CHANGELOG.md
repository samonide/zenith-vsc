# Change Log

All notable changes to the Zenith Theme extension will be documented in this file.

## [6.0.0] - 2026-02-01

### 🎉 Major Release - Base46 Architecture

This is a complete redesign of Zenith based on the **base46 color architecture**, bringing industry-standard theming and universal compatibility.

### ✨ New Features
- **Complete redesign** using base46 color system from the main Zenith repository
- **Eight unique variants** - added Twilight (rose tones) replacing old color scheme
- **Synchronized colors** with the main Zenith repo for cross-platform consistency
- **Enhanced syntax highlighting** with better token differentiation using base_16 colors
- **Panel transparency** - panels are now transparent with borders only on terminal (matching standard themes)
- **Professional UI** - improved borders, selections, and visual hierarchy throughout
- **Better text selection** - more visible selection highlighting across all themes
- **Improved terminal** - better ANSI color mapping for accurate terminal rendering

### 🎨 Theme Changes
- 🌙 **Dusk** - Flagship theme with perfectly balanced soft pastels
- ☀️ **Dawn** - Elegant light theme (fully redesigned)
- ✨ **Aurora** - Ethereal teals and dreamy lavenders (enhanced)
- 🌸 **Twilight** - NEW! Warm rose-tinted theme (formerly named Rosé in base repo)
- 🌊 **Ocean** - Deep serene blues and aqua tones (enhanced)
- 🌲 **Forest** - Natural vibrant greens (enhanced)
- 🌑 **Midnight** - Pure deep darkness with high contrast (enhanced)
- 🧘 **Monochrome** - Ultra-minimal monochrome (renamed from Zen for clarity)

### 🔧 Technical Improvements
- Automated theme generation from base46 JSON files
- Consistent color mapping across all variants
- Better adherence to VS Code theme guidelines
- Improved semantic highlighting support
- Enhanced diff editor colors
- Better debug UI integration

### 🎯 UI Enhancements
- More consistent border usage (transparent panels with terminal border)
- Better active/inactive state differentiation
- Improved hover states throughout UI
- Enhanced peek view styling
- Better notification styling
- Improved search result highlighting

### 📝 Breaking Changes
- Color values have changed across all themes due to base46 architecture
- Panel backgrounds are now transparent (matching standard VS Code themes)
- Some theme-specific colors may appear different but are more consistent

---

## [5.1.2] - 2026-01-29

### 🎨 Improved
- **Zenith Forest:** Significantly increased keyword contrast (20%+ improvement)
  - Brightened accent green from #6ec095 → #8be5b8 for much better visibility
  - Keywords now clearly stand out from background green tones
  - Improved differentiation between syntax elements

## [5.1.1] - 2026-01-29

### 🎨 Improved
- **Zenith Aurora:** Significantly improved contrast and readability
  - Brightened foreground colors (#e5f2f5)
  - Enhanced accent color visibility (#d0a5c0)
  - Better keyword differentiation with cyan tones (#8fc5c3)
  - Slightly lighter background for improved text clarity
- **Zenith Forest:** Enhanced visibility and contrast
  - Brightened foreground (#c8d7cf) for better readability
  - More vibrant accent green (#6ec095)
  - Improved blue tones (#75a0c0) for better syntax distinction
  - Adjusted background lightness for reduced eye strain
- Both themes now have much clearer keyword and syntax element visibility

## [5.1.0] - 2026-01-29

### 🐛 Bug Fixes
- **CRITICAL:** Fixed text selection visibility - selected text is now clearly visible with distinct highlighting
- Improved inactive selection contrast for better multi-cursor editing experience

### ✨ UX Enhancements
Refined the theme with modern improvements inspired by popular themes like Catppuccin and Tokyo Night:
- **Editor:** Enhanced bracket matching with colorful bracket pair highlighting
- **Editor:** Better cursor and active line number coloring using theme accent
- **Editor:** Improved word highlight borders for better visual distinction
- **Editor:** Enhanced find/replace match highlighting with visible borders
- **Scrollbar:** More visible scrollbar with theme-colored active state
- **Lists:** Better selection contrast and hover states throughout the UI
- **Tabs:** Active tabs now use accent color for better distinction
- **Tabs:** Added hover states and better unfocused tab styling
- **Widgets:** Refined borders on autocomplete, hover widgets, and suggestions
- **Widgets:** Added icon coloring in suggestion lists
- **Indent Guides:** Active indent guide now uses theme accent color
- **Peek View:** Enhanced with better borders and match highlighting
- Overall improved contrast and visual hierarchy across all UI elements

### 🎨 Visual Improvements
- More consistent use of theme accent colors throughout the interface
- Better visual feedback for interactive elements
- Subtle shadows and borders for improved depth perception
- Enhanced color consistency with the Zenith design philosophy

## [5.0.1] - 2026-01-15

### 🎉 Major Update - Zenith v5.0.1

**Breaking Changes:**
- Complete refactorization of color system based on upstream Zenith v5.0.1
- Removed **Zenith Midnight** variant
- Added **Zenith Aurora** variant - soft northern lights theme with gentle teals, pinks, and purples

### Changed
- Rebuilt all themes using new unified color structure from Zenith v5.0.1
- Improved color consistency across all variants
- Enhanced semantic token mappings
- Better syntax highlighting accuracy
- Updated all UI colors to match new color palette

### Technical
- Created automated theme generator script for easier maintenance
- Aligned with upstream Zenith color definitions
- All themes now generated from `colors-*.json` source files

## [3.0.2] - 2026-01-01

### Improved
- Enhanced context menu (right-click menu) styling to match theme colors
- Added proper theming for menu backgrounds, selection states, and borders
- Improved visual consistency across all 6 theme variants

## [3.0.0] - 2025-01-01

### Added
- 🎉 Initial release of Zenith Theme for VS Code
- 6 beautiful theme variants:
  - Zenith Dusk (Default dark theme)
  - Zenith Dawn (Light theme)
  - Zenith Twilight (Deeper dark theme)
  - Zenith Forest (Earthy green-gray dark theme)
  - Zenith Retro (Vintage warm dark theme)
  - Zenith Ocean (Deep blue dark theme)
- Complete VS Code UI theming for all variants
- Semantic highlighting support
- Rich syntax highlighting for all major languages
- Terminal color support
- Git decoration colors
- Full editor widget theming

### Features
- Soft pastel color palette designed for eye comfort
- Consistent design language across all variants
- Optimized for long coding sessions
- High readability with proper contrast
- Beautiful UI integration

---

## Roadmap

### Upcoming Features
- [ ] Additional theme customization options
- [ ] More language-specific highlighting improvements
- [ ] Community feedback integration
- [ ] Performance optimizations
- [ ] Enhanced semantic token support

---

Check [Releases](https://github.com/samonide/zenith-vsc/releases) for detailed information about each version.
