### Color Text based on class

```lua
function ()
    for unit in WA_IterateGroupMembers(forceParty) do -- Iterates through group members
        if WA_GetUnitAura(unit, 425153, "HELPFUL") then -- Unit, SpellID, Filter
	        -- pass unitName through class color function and return
            return WA_ClassColorName(aura_env.state.unitName)
        end
    end
end
```
