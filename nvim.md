# 🧠 My Neovim Configuration

This is my personal [Neovim](https://neovim.io/) setup, based on the excellent [kickstart.nvim](https://github.com/nvim-lua/kickstart.nvim) starter configuration.

> 🔗 Repo: [RafaelAndeloci/kickstart.nvim](https://github.com/RafaelAndeloci/kickstart.nvim)

## 🛠 Features

- ⚡ Powered by [Lazy.nvim](https://github.com/folke/lazy.nvim) plugin manager  
- 🎨 Custom statusline using [lualine.nvim](https://github.com/nvim-lualine/lualine.nvim)  
- 🧩 Modular plugin config (separated files for better structure)  
- 💡 LSP, Treesitter, file explorer, git integration, and more  

## 📦 Notable Plugins

| Plugin           | Description                      |
|------------------|----------------------------------|
| `lualine.nvim`   | Fast and configurable statusline |
| `telescope.nvim` | Fuzzy finder for files, LSP, etc |
| `nvim-tree.lua`  | File explorer tree               |
| `nvim-cmp`       | Completion engine                |
| `mason.nvim`     | Manage LSP/DAP servers easily    |

## 📁 Plugin Structure

Plugin configurations are placed in the `lua/custom/plugins/` directory.  
For example:

```lua
-- ~/.config/nvim/lua/custom/plugins/lualine.lua
return {
  'nvim-lualine/lualine.nvim',
  dependencies = { 'nvim-tree/nvim-web-devicons' },
  config = function()
    require('lualine').setup {
      options = {
        theme = 'auto',
        section_separators = '',
        component_separators = '',
      },
    }
  end,
}
```

Then loaded via:

```lua
-- ~/.config/nvim/lua/custom/plugins/init.lua
return {
  require("custom.plugins.lualine"),
  -- other plugin configs
}
```

## 🚀 Getting Started

Clone the repository:

```bash
git clone https://github.com/RafaelAndeloci/kickstart.nvim ~/.config/nvim
nvim
```

Neovim will install all plugins on the first run.

---

Feel free to fork or explore the config to build your own!
