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
* Below is an example of how to set the setup properly.

```lua
require...({
  keybinds = {
    ["<leader>jb"] = "JavaBuild" -- Building all Java Files in src directory in.
    ["<leader>jr"] = "JavaRun" -- Runs Main.java in the out folder in your project_root
    ["<leader>nf"] = "NewJavaFile" -- Creates a new Java file in the current project src folder
    ["<leader>np"] = "NewJavaProject" -- Creates a new project in the project directory in the config, defaults to ~/Projects
  }
})
```
