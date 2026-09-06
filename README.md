
# 🛠️ Hyprland Dotfiles

A minimalist, high-performance Wayland environment configured for productivity, bare-metal development, and low-latency workflows on Arch Linux / CachyOS.

---

## 📸 Overview & Key Components

| Category | Component | Description |
| :--- | :--- | :--- |
| **Window Manager** | [Hyprland](https://hyprland.org/) | Dynamic tiling Wayland compositor |
| **Status Bar** | [Waybar](https://github.com/Alexays/Waybar) | Highly customizable GTK status bar |
| **App Launcher** | [Fuzzel](https://codeberg.org/dnkl/fuzzel) | Wayland-native application launcher |
| **Terminals** | [Ghostty](https://ghostty.org/) / [Kitty](https://sw.kovidgoyal.net/kitty/) | GPU-accelerated terminal emulators |
| **Text Editor** | [Neovim](https://neovim.io/) | Extensible terminal-based code editor |
| **System Monitor** | `btop` / `htop` | Process and resource tracking |
| **Theming** | `qt5ct` / `qt6ct` / `Kvantum` | Unified GTK & Qt application styles |

---

## 📂 Repository Structure

```text
.
├── hypr/        # Hyprland bindings, keymaps, and window rules
├── waybar/      # Status bar layout and CSS styling
├── fuzzel/      # Launcher keybindings and color themes
├── ghostty/     # GPU terminal configurations
├── kitty/       # Terminal font & color settings
├── nvim/        # Neovim plugins and LSP configurations
├── rofi/        # Fallback runner configurations
├── gtk-3.0/     # GTK3 dark theme overrides
├── gtk-4.0/     # GTK4 dark theme overrides
└── Kvantum/     # SVG-based theme engine configs

```

---

## 🚀 Quick Setup & Installation

> [!WARNING]
> Backup your existing configurations in `~/.config/` before linking these files.

1. **Clone the repository:**
```zsh
git clone ssh://git@ssh.github.com:443/norbertsawe/hyprland-dotfiles.git ~/.config/hypr-dots

```


2. **Symlink key configuration directories:**
```zsh
ln -s ~/.config/hypr-dots/hypr ~/.config/hypr
ln -s ~/.config/hypr-dots/waybar ~/.config/waybar
ln -s ~/.config/hypr-dots/fuzzel ~/.config/fuzzel
ln -s ~/.config/hypr-dots/ghostty ~/.config/ghostty
ln -s ~/.config/hypr-dots/kitty ~/.config/kitty
ln -s ~/.config/hypr-dots/nvim ~/.config/nvim

```


3. **Reload Hyprland:**
Press `SUPER + SHIFT + R` or execute `hyprctl reload` in your terminal.

