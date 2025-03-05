# Installation
!!! Javanvim can be installed with any plugin installer or manually. These are just examples.

## Lazyvim
----------

```lua
require {
  "DarthMooMancer/Javanvim",
  config = function()
    require("Javanvim").setup()
  end
}
```

## Mini.Deps
------------
```lua
MiniDeps.add({ source = 'DarthMooMancer/Javanvim', name = "Javanvim" })
require("Javanvim").setup()
```

