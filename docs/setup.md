# Setup and Customizing

## Project Name

```lua
require("Javanvim").setup({
  project_root = "~/Home/..." -- Default: ~/Projects
})
```

* You can change the default directory for the project. The project can be made from anywhere you want.
* It will automatically make the new Root Directory, so you don't have to worry about making it.

## Keybinds
```lua
-- These are defaults, so no need to copy them
require("Javanvim").setup({
  keybinds = {
    ["<leader>jb"] = "JavaBuild" -- Building all Java Files in src directory in.
    ["<leader>jr"] = "JavaRun" -- Runs Main.java in the out folder in your project_root
    ["<leader>nf"] = "NewJavaFile" -- Creates a new Java file in the current project src folder
    ["<leader>np"] = "NewJavaProject" -- Creates a new project in the project directory in the config, defaults to ~/Projects unless project_root is set
    ["<Esc>"] = "CloseTerminal" -- Closes terminal, esc by default. 
  }
})
```

## Terminal

* The terminal has a couple of options that can be customized and with more to come
    - Each is set to 0 by default
        * **_right_padding:_** Padding for the right width of the terminal
        * **_left_padding:_** Padding for the left width of the terminal
        * **_top_padding:_** Padding for the top height of the terminal
        * **_bottom_padding:_** Padding for the bottom padding of the terminal
    - Each is enabled by default
        * **_border:_** Adds a rounded border to the window
        * **_number:_** Adds numbers to side of terminal
        * **_relativenumber:_** Relative numbers indicate distances from the cursor, only works if number is enabled
        * **_scroll:_** Allows scrolling in terminal

```lua
-- These are just defaults, so no need to copy them
require("Javanvim").setup({
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
```
