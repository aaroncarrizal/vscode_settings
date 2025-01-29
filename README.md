# VS Code Configuration Guide

This repository contains a VS Code settings JSON file with various customizations for an optimized coding experience. Below is an explanation of the key configurations.

## General Editor Settings

- 🎨 **Font & Ligatures**
  - `editor.fontFamily`: "Fira Code" (a monospaced font with programming ligatures)
  - `editor.fontSize`: 14 (sets the font size)
  - `editor.fontLigatures`: `true` (enables font ligatures for better code readability)

- ✍️ **Cursor & Navigation**
  - `editor.cursorSmoothCaretAnimation`: "on" (smooth cursor animation)
  - `editor.cursorBlinking`: "expand" (cursor blinking animation style)
  - `editor.bracketPairColorization.enabled`: `true` (enables bracket pair colorization for better visibility)
  - `editor.wordWrap`: "on" (ensures long lines wrap instead of scrolling horizontally)

- 🖥️ **Minimap & UI Tweaks**
  - `editor.minimap.enabled`: `false` (disables minimap for a cleaner UI)
  - `breadcrumbs.enabled`: `false` (hides breadcrumbs navigation)
  - `window.commandCenter`: `true` (enables the command center for quick access to commands)

## Formatting & Prettier

- 🛠️ **Default Formatter**
  - `editor.defaultFormatter`: `esbenp.prettier-vscode` (sets Prettier as the default formatter)
  - `editor.formatOnSave`: `true` (automatically formats files on save)
- 📏 **Prettier Rules**
  - `prettier.bracketSameLine`: `true` (keeps brackets on the same line for JSX/HTML elements)
  - `prettier.tabWidth`: `4` (sets indentation width to 4 spaces)
  - `prettier.semi`: `false` (removes semicolons at the end of statements)
  - `prettier.trailingComma`: `none` (disables trailing commas)
  - `prettier.bracketSpacing`: `true` (adds spaces inside object literals)
  - `prettier.singleAttributePerLine`: `false` (allows multiple attributes per line in JSX/HTML)
  - `prettier.singleQuote`: `true` (enforces single quotes)

## Workbench & UI Customizations

- 🎭 **Layout & Themes**
  - `workbench.editor.splitInGroupLayout`: "vertical" (sets split editor layout to vertical)
  - `workbench.colorTheme`: "GitHub Dark" (active color theme)
  - `workbench.startupEditor`: "none" (prevents opening the welcome page at startup)
  - `workbench.iconTheme`: "material-icon-theme" (sets the icon theme to Material Icons)
- 🎨 **Custom Colors**
  - `workbench.colorCustomizations`: Customizes background colors for various UI elements when using "One Dark Pro Darker" theme.

## Terminal & Git Settings

- 💻 **Terminal Customizations**
  - `terminal.integrated.fontFamily`: "Fira Code" (matches the editor font for consistency)
  - `terminal.integrated.cursorStyle`: "line" (sets cursor style in the terminal)
  - `terminal.integrated.enableMultiLinePasteWarning`: `false` (disables paste warning)

- 🔄 **Git Configuration**
  - `git.autofetch`: `true` (automatically fetches changes from remote repositories)
  - `git.confirmSync`: `false` (disables confirmation prompt when syncing changes)

## File & Explorer Behavior

- 💾 **Auto Save & Formatting**
  - `files.autoSave`: "afterDelay" (auto-saves files after inactivity)
  - `files.autoSaveDelay`: `1500` (sets auto-save delay to 1.5 seconds)
  - `files.trimTrailingWhitespace`: `true` (removes trailing whitespace on save)
- 🗂️ **Explorer & Deletion**
  - `explorer.confirmDelete`: `false` (disables delete confirmation for quicker file removal)

## Language-Specific Settings

- ⚡ **Emmet Enhancements**
  - `emmet.includeLanguages`: Maps JavaScript to JavaScript React and Vue HTML to standard HTML for Emmet support.

- 📝 **Formatter per Language**
  - `[javascript]`: Uses VS Code's built-in TypeScript formatter.
  - `[html]`: Uses VS Code's built-in HTML formatter.

## Remote & Database Features

- 🌍 **Database & Remote Development**
  - `database-client.autoSync`: `true` (automatically syncs database changes)
  - `remote.autoForwardPortsSource`: "hybrid" (automatically forwards ports for remote development)

## Accessibility

- 🔔 **Task Completion Sound**
  - `accessibility.signals.taskCompleted.sound`: "on" (enables sound notifications for completed tasks)

---

### How to Use These Settings

1. 📂 Copy the JSON file into your VS Code `settings.json`.
2. 🔄 Restart VS Code for changes to take effect.
3. ✏️ Customize further according to your preferences!

---

### How to Install Recommended Extensions

1. 🔍 Open VS Code and navigate to the Extensions panel (`Ctrl+Shift+X` or `Cmd+Shift+X` on macOS).
2. ⚙️ Click on the `...` menu in the top right corner of the Extensions panel.
3. ✅ Select `Show Recommended Extensions`.
4. 📥 Install all recommended extensions manually or individually.

Alternatively, if you want to install all extensions via the terminal, run:

```sh
cat extensions.txt | xargs -L 1 code --install-extension
```

---

### Custom Keybindings

These are some useful keybindings configured for a more efficient workflow:

- ⌨️ **Editor Commands**
  - `Ctrl+Tab`: Delete the current line.
  - `Ctrl+Shift+K`: (Removed default delete line binding).
  - `Ctrl+Shift+C`: Block comment.
  - `Ctrl+Shift+X`: Toggle line comment.

- 🖥️ **Terminal Shortcuts**
  - `Ctrl+Shift+T`: Open a new terminal.
  - `Ctrl+Shift+T` (when terminal is focused): Split terminal.
  - `Ctrl+T`: Toggle terminal visibility.
  - `Ctrl+Shift+5`: (Removed default split terminal binding).
  - `Ctrl+Shift+\``: (Removed default new terminal binding).

- 🔄 **Other Changes**
  - `Ctrl+Tab`: (Removed quick switch between recent editors).
  - `Ctrl+Shift+X`: (Removed extensions view binding).
  - `Ctrl+Shift+T`: (Removed reopen closed editor binding).
  