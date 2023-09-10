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

# Excusing & Whitelisting

To excuse a player for a particular amount of time, you can use the `Excuse` function of Genesis. Refer to the figure below:

```lua
local Excuse = Genesis.Excuse
local Player = game.Players.Mlgisbetter -- Insert player here

Excuse(Player, 50) -- Second argument is the amt of time
```

# Ragdoll Support

If you have ragdolls in your game and you would like to add Ragdoll support, go into the "Configuration" module listed under Genesis, and add the function "Ragdoll" in the table. The function should return a boolean that determines whether or not a player is currently ragdolled. For example, the function could look like this:

```lua
Ragdoll = function(Character: Model) : boolean?
  return Character:FindFirstChildOfClass('BallSocketConstraint', true) and true
end)
```

# Why Not Client?

Client-based anticheats are generally unfavorable. Not only that, but with the efforts of the hundreds of exploiters online can easily bypass a client-based anticheat. 
Overall, The client is not to be trusted, as they have the power to manipulate properties, functions, and more. 
Server-sided anticheats provide a solution to this, in that they have full control over themselves; cheaters cannot do anything to pause or stop a server-sided anticheat.
