# 🛠 Rafael Andeloci's Dotfiles

Welcome to my dotfiles! This repository contains the configuration files and personal setup I use for my development environment across Linux and Windows systems.

> ✨ These dotfiles are built for productivity, minimalism, and full control over my tools.

## 📁 Repositories

| Tool/Area       | Repository                                                                 |
|-----------------|-----------------------------------------------------------------------------|
| 🧠 Neovim        | [kickstart.nvim](https://github.com/RafaelAndeloci/kickstart.nvim)         |
| 🖥️ Terminal      | This repo (Zsh, aliases, tmux, starship, etc.)                            |
| 🧰 Git config    | Included in this repo as `.gitconfig`                                     |
| 🔧 System setup  | Shell scripts to bootstrap packages and configs (e.g. `setup.sh`)         |

---

## 🧠 Neovim

My Neovim configuration is based on [kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim), but extended with custom plugin configurations, LSPs, and personal preferences.

> 📦 Statusline using [lualine.nvim](https://github.com/nvim-lualine/lualine.nvim) is configured separately in `lua/custom/plugins/lualine.lua`.

See the full config here:  
🔗 **[RafaelAndeloci/kickstart.nvim](https://github.com/RafaelAndeloci/kickstart.nvim)**

## 🖥️ Terminal (Zsh, Starship, Tmux)

This repository includes configuration for:

- **Zsh** (`.zshrc`) with custom aliases and plugin loader
- **Starship prompt** (`starship.toml`) for a fast, informative prompt
- **Tmux** (`.tmux.conf`) with sensible defaults and vi-mode
- **Custom scripts** (in `bin/` or `scripts/` if present)

## 🔧 Git Config

My global Git configuration is tracked in `.gitconfig` and includes:

- Custom aliases (`co`, `br`, `st`, etc.)
- Merge and diff tools
- Name/email identity

## 🚀 Getting Started

To use these dotfiles:

```bash
git clone https://github.com/RafaelAndeloci/dotfiles ~/.dotfiles
cd ~/.dotfiles
./setup.sh
```

> 📝 You may need to manually symlink or source `.zshrc`, `.gitconfig`, etc., depending on your setup strategy.

---

## 💡 Philosophy

These dotfiles are meant to be:

- **Modular** – Easy to understand and extend
- **Minimal** – No heavy dependencies or frameworks
- **Portable** – Work across Linux systems with few adjustments

---

## 📸 Screenshots (optional)

_Add a screenshot of your terminal + Neovim here if you'd like!_

---

## 📜 License

MIT License — feel free to copy, fork, and adapt.
