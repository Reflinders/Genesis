# Genesis
Genesis is a server-sided anticheat focused on the principal physics-based exploits

# Starting

Starting up Genesis is quite simple; all you have to do is call the `Manage` function, and import the needed modules (Charcoal, Waves) into your game.

```lua
local Genesis = require(GenesisModule)
Genesis.Manage()
```

# Quitting

To quit Genesis, simply call the `Quit` function:

```lua
Genesis.Quit()
```

# Features

Genesis has 4 fundamental anti-exploits — Basic Movement (jumping, walking), Flying, Anti-gravity, and Noclip.
In the future, I plan on adding a couple more.

# Why Not Client?

Client-based anticheats are generally unfavorable. Not only that, but with the efforts of the hundreds of exploiters online can easily bypass a client-based anticheat. 
Overall, The client is not to be trusted, as they have the power to manipulate properties, functions, and more. 
Server-sided anticheats provide a solution to this, in that they have full control over themselves; cheaters cannot do anything to pause or stop a server-sided anticheat.
