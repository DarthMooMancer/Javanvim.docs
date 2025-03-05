## An example of Lazyvim and setup
------------
::: warning
Quick note: There is no need to copy this. This is an example, but it consists of the defaults.
:::

```lua
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
        width_pad = 10,
        height_pad = 10,
        border = true,
        number = true,
        relativenumber = true,
        scroll = true,
      }
    })
  end
}
```
