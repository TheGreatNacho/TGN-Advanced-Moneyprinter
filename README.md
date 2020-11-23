
TheGreatNacho's Advanced Moneyprinter for DarkRP:
============================================
This pack has three different sized batteries, an overclocker, a cooler, a failsafe and the actual printer.

 - The batteries add power to the printer, not upgrade the battery size.There's a button for that if you press E on the printer.
 - The overclocker makes the money printer print faster and collect XP faster, but will cause the printer to over heat faster.
 - The cooler keeps the money printer cool and keeps the slows the printers over heat bar.
 - The fail safe stops the printer from over heating by shutting it off at the point you program into the failsafe (by pressing E while looking at the failsafe) You can have more the one fail safe in a printer at once because there is a chance your fail safe will... fail... hehe...

The entities you want to add to your entities list are;
```adv_moneyprinter
printer_smallbattery
printer_mediumbattery

printer_largebattery
printer_overclocker
printer_cooler
printer_failsafe
```

## Installation:
For a proper understanding of how the entities.lua works, see [The DarkRP Wiki](https://darkrp.miraheze.org/wiki/DarkRP:CustomEntityFields)
1. Copy the addon into your `garrysmod/addons` folder.
2. Open the darkrp entities.lua in `garrysmod/addons/darkrpmodification/lua/darkrp_customthings/`
3. For each of the entities listed above, create an entity in the entities.lua

For the lazy people, you can copy this straight into your entities.lua, and modify it how you please.
```
DarkRP.createEntity("Money Printer", {
        ent = "adv_moneyprinter",
        model = "models/props_c17/consolebox01a.mdl",
        price = 7500,
        max = 3,
        cmd = "buyprinter"
})
DarkRP.createEntity("Printer Cooler", {
        ent = "printer_cooler",
        model = "models/props_c17/consolebox01a.mdl",
        price = 5000,
        max = 3,
        cmd = "buycooler"
})
DarkRP.createEntity("Printer Failsafe", {
        ent = "printer_failsafe",
        model = "models/props_c17/consolebox01a.mdl",
        price = 3000,
        max = 3,
        cmd = "buyfailsafe"
})
DarkRP.createEntity("Printer Overclocker", {
        ent = "printer_overclocker",
        model = "models/props_c17/consolebox01a.mdl",
        price = 3000,
        max = 3,
        cmd = "buyoverclocker"
})
/*
DarkRP.createEntity("Small Battery", {
        ent = "printer_smallbattery",
        model = "models/props_c17/consolebox05a.mdl",
        price = 500,
        max = 6,
        cmd = "buysbattery"
})
DarkRP.createEntity("Medium Battery", {
        ent = "printer_mediumbattery",
        model = "models/props_c17/consolebox05a.mdl",
        price = 1000,
        max = 6,
        cmd = "buymbattery"
})
DarkRP.createEntity("Large Battery", {
        ent = "printer_largebattery",
        model = "models/props_c17/consolebox05a.mdl",
        price = 2500,
        max = 6,
        cmd = "buylbattery"
})
```