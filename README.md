# rust-primitive
Facepunch Rust private server configuration. 
Real scarcity survival primitive medieval solo/duo inspired by Mountain Men TV Series. 

## Server philosophy
Removed most high tech gears, weapons and kept primitive items to keep the game slow and challenging.  Reduce plant growth, spawn rate. Adjusted animal loot table so each animal plays a role either cloth, leather, meat, etc.  Added some default blueprint for everyone and removed ones related to advance items. 

## Server configuration
From [cfg/server.cfg](cfg/server.cfg) file 
server.pvp true  
server.pve false  
sleepers.on true  
truth.enforce true  
minicopter.population 0  
heli.lifetimeMinutes "0"  
server.planttick "480"  
bradley.enabled false  
cargoship.event_enabled false  
decay.upkeep_period_minutes "9999"  
decay.upkeep_grief_protection "2880"  
spawn.min_rate ".1"  
spawn.max_rate ".3"  
spawn.min_density ".1"  
spawn.max_density ".3"  
server.seed true  
server.worldsize 6000  
server.seed 2068376  
bear.population "4"  
boar.population "8"  
chicken.population "9"  
horse.population "4"  
wolf.population "5"  
stag.population "6"  
o.grant group default blueprintmanager.conf  

## Thrid Party add-on used
Oxide now known as umod https://umod.org/plugin is used to create this custom server. 

### Better Loot
Desc : Instead of using the game's default loot tables, Better Loot overrides any barrels and crates a player loots with something (hopefully) better.
Plugin from https://umod.org/plugins/better-loot
Config file is [oxide/config/BetterLoot.json](oxide/config/BetterLoot.json)
Used https://blmc.artemdanilkin.ru/ to create custom loot for crates

### Blue Print Manager
Desc : Allows you to grant all blueprints, reset blueprints, and grant specific blueprints.
Plugin from https://umod.org/plugins/blueprint-manager
Config file is [oxide/config/BlueprintManager.json](oxide/config/BlueprintManager.json)


### Component Blocker
Desc : Removes entities and items completely from the game. This plugin is for server owners who want to restrict the availability of items or entities in the game world
Plugin from https://umod.org/plugins/component-blocker 
Config file is [oxide/config/ComponentBlocker.json](oxide/config/ComponentBlocker.json)

### Gather manager 
Desc : Allows for modification the amount of resources people gain from gathering them from dispensers, the amount gained from using a Mining Quarry, the amount gained from using Survey Charges when they are successful, and the amount of the collectible object pickups (the small lootable rocks and wood logs on the ground scattered around the map).
Plugin from https://umod.org/community/gather-manager
File is [oxide/config/GatherManager.json](oxide/config/GatherManager.json)

### Metabolism
Desc : Allows you to change or disable the default metabolism values such as health, calories, and water (hydration) for all players with the related permission
Plugin from https://umod.org/plugins/metabolism
Config file is [oxide/config/Metabolism.json](oxide/config/Metabolism.json)
