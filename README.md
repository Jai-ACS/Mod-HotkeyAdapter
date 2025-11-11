# Mobile Key Bridge
Mod that helps bridge mods that require keyboard shortcut to use. This allows mods that originally require keyboard (usually to launch a configuration dialog). This mod provides an extra button in the menu where bridged mods could be launched.

# Interfacing
In order for your mod to be bridged, you need to interface your mod with this bridge.

```Lua
local Bridge = GameMain:GetMod("Jai_MobileKeyBridge")
...
...
Bridge:register("Mod Name", "Function Name",
	function()
		-- This is executed when the user taps on this feature
	end
)
```
