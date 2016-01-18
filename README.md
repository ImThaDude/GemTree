# GemTree
This is GemTree, a stat tree based on gems within game

GemTree is a plugin that creates and executes the statistics within an item in minecraft.
GemBase can be created by putting 2 diamonds in a shapeless form.
The player can then use this gem and place it in their Gem inventory.
Players will get status boost by this Gems. This is because I want to keep the vanilla weapons.
Weapons might be implemented later.
Or maybe special Gems which will let the player have a stat boost while wielding the weapon.
There will also be gems that will give an aura if the player uses the same type of gem.

The GemBase can be updated to a higher stat item as the player upgrades it more and more.
To upgrade it players can go to a gem blacksmith and the blacksmith will request for ingredients.
The blacksmith will only show upgrades for the gems you currently have on inventory.

Gems can be placed on a gem inventory through maybe a box or a command.
The player will place the gems and as soon as the player exits, the player stats will be upgraded.
Therefore the server does not have to load every time. Instead there is a fixed object which will have
the stats of the player. Or maybe change the base stats. With this the server can easily calculate the level of
the player. Players with lower levels will be informed when there is a player of higher level within 50 blocks.
Players with higher level will have different colored names.

There are two files on GemTree. The tree yml is the upgrade path for the item. The server will load this tree
and therefore will find the next upgrade. Maybe create a custom tree object? Maybe add all of the items on an arraylist
and add the upgrade properties in them. It clears it and refreshes it every time the server is loaded. Traverse through stats!
Because the items should inherit their last stats. Maybe create IDs based on tree? Gem Tree will also create a tree to see through
a yml

GemTree:
    BASE01: ##Base Gem
        DMG001: ## +1 Dmg
            DMG002: ## +2 Dmg
                DMG003: ## +3 Dmg
                    DMG004: ## +4 Dmg
                        DMG005: ## +5 Dmg
            KNGT01: ## +1 Dmg & +1 Penetration
                KNGT02: ## +2 Dmg & 1 Pen
                    KNGT02: ## +2 Dmg & +2 Pen
                        KNGT03: ## +3 Dmg & +2 Pen


The currently config yml will contain the status effects inside of the file.

GemStats:
    BASE01:
        Name: Base Gem
        Stats:
            Health: 1
        Recipee:
            2 Diamonds
    DMG001:
        Name: Zombie Harth
        Stats:
            Damage: 1
        Recipee:
            2 Zombie Guts
    DMG001:
        Name: Zombie Harth II
        Stats:
            Damage: 2
        Recipee:
            2 Great Zombie Guts
          
To get the gem items players have to craft based on the items requested. Also, in order to make it easier. Anything
that has a great on it is a boss. Anything that has Big Great is a bigger zombie boss.

There can also be legendary branches for gems that are rarely or dropped by bosses. This branches will be cheaper than normal
but they will be temporal. They have special powers and stuff. They can be updated and stuff. It will contain odd stats.

The reason it will not be a crafting system it is because its too complicated to make our players learn all recipees for every
upgrade.

Legendaries can use chain as gear. Or anything. More specific on what the player has to wear to work.

Players can decide to upgrade their gems in the same tier. This is called Enhance. Enhance will increase the stats of a Gem temporally
For every monster there will be an item which will let you enhance it several levels. The inside the items specifically will have an enhance thing. So players can update with no guilt their items. This will be called enhance dust.

When you get a legendary, It will drop as an ancient gem, it will say. Its barely readable. Players can take this gem
and polish it therefore the gem will be spawned as a gem. instead of hardcoded.
code.
