### Lazyvim and Config
```lua
-- There is no need to copy this. This is an example and it consists of the defaults.
require {
  "DarthMooMancer/Javanvim",
  config = function()
    require("Javanvim").setup({
      project_root = "~/projects",
      keybinds = {
        ["<Esc>"] = "CloseTerminal",
        ["<leader>jb"] = "JavaBuild",
        ["<leader>jr"] = "JavaRun",
        ["<leader>nf"] = "NewJavaFile",
        ["<leader>np"] = "NewJavaProject",
      },
      terminal = {
        right_padding = 0,
        bottom_padding = 0,
        left_padding = 0,
        top_padding = 0,
        border = true,
        number = true,
        relativenumber = true,
        scroll = true,
      }
    })
  end
}
```
