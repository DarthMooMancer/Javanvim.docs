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
* !!! There is currently an error with the keybinds, the main keybinds are used however the defaults are not overwritten. I am trying to find a fix, but it may be some time before I can fix the issue. So there are 2 keybinds that can be used if you set on in the init.lua. The only one that works as intended is CloseTerminal.
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

- The terminal has a couple of options that can be customized and with more to come

* width_pad - 10 by default, padding for the width of the terminal
* height_pad - 10 by default, padding for the width of the terminal
* border - true by default
* number - true by default, adds numbers to side of terminal
* relativenumber - true by default, only works if number is enabled also
* scroll - true by default, allows scrolling in terminal

* Below is an example of how to set the setup properly:
```lua
require...({
  terminal = {
    width_pad = 0,
    height_pad = 0,
    border = false,
    number = false, -- if number is false, no need to make relativenumber false as well
    scroll = true,
  }
})
```
