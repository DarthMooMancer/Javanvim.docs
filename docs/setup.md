# Setup and Customizing

## Project Name

```lua
require...({
  project_root = "~/Home/..." -- Default: ~/Projects
})
```

* You can change the default directory for the project. The project can be made anywhere you want.
* It will automatically make the new Root Directory, so you don't have to worry about that.

## Keybinds
* The default keybinds are below so you don't need to worry about setting them up. 
* Below is an example of how to set the setup properly:

```lua
require...({
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

  * right_padding - 0 by default, padding for the right width of the terminal
  * left_padding - 0 by default, padding for the left width of the terminal
  * top_padding - 0 by default, padding for the top height of the terminal
  * bottom_padding - 0 by default, padding for the bottom padding of the terminal
  * border - true by default
  * number - true by default, adds numbers to side of terminal
  * relativenumber - true by default, only works if number is enabled also
  * scroll - true by default, allows scrolling in terminal

* Below is an example of how to set the setup properly:
```lua
require...({
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
