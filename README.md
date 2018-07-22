# OFTRTA-poe-filter

[Loot Filter] One Filter to Rule Them All for Path Of Exile

## Disclaimer

Those filters are not my work, all credits go to Florian Thießen. The goal of this repository is archiving, easier access and easier way to fork to create modified filters. I'll have my modified version on other branches.

Original Path of Exile [forum thread](http://www.pathofexile.com/forum/view-thread/1259059).

## How to install?

Put teh scripts in `C:/User/Your_Username/Documents/My Games/Path of Exile/`.

It will now appear ingame in the options panel (press `O`) at the end of the `UI` tab.

There's also a well made [video](https://www.youtube.com/watch?v=KY1x92eibB0) by [EngineeringEternity](https://www.pathofexile.com/account/view-profile/EngineeringEternity).

## Features / Ideas

- One filter to cover everything from leveling to racing and endgame content without compromise.
- Sane defaults while offering all the options in the world for those that like to customize.
- Be easy on the eyes, default colors look nice so let's use them where we can.
- Smooth integration, no learning period, be intuitive.
- Highlight stuff that is worth highlighting. Most of the items are hidden anyway, so there's no need to go over board.

## More specific

Highlight/Show:

- really rare items (Mirror, Fishing Rod, ...) in stark colors
- 6L, 5L, 6S
- Chromatics with a slight green border
- Chisel recipe items (Gavel, Stone Hammer and Rock Breaker) with a grey bordercolor
- Rare currency (Eternal, Exalt, Divine) with a unique bordercolor
- Gems with 10+ quality by adding a border in the default gem color
- Maps that are level 74+/79+
- Prefered chaos/regal recipe items
- Rare jewellery (rings, amulets, belts) with a rare border
- 3L Quartz / Crystal Sceptre with a stark red border during lvling
- Quality Flasks in a slightly brighter font
- T1 Armour (normal/magic) with 3/4 sockets; >= 79/84 in a slightly brighter font / background
- T1 Weapons (normal/magic) with 3/4 sockets; >= 79/84 in a slightly brighter font / background
- Highest available rare item tier based on zone level with a rare bordercolor
- Rare T1 Armour, Weapons and Craft bases with an itemlevel >= 79/84

## Change behavior based on zone level

During leveling you will see less and less normal/magic items as you progress. Generally normal and magic items are shown as long as they are appropriate for the current zone.
By default items need a certain amount of sockets to be shown to reduce clutter. This can be modified using the various toggles existing in the script.

Rare items are highlighted if their basetype is the currently highest available.
Example: You are in a level 21 zone and a rare "Recurve Bow" (DropLevel = 20) drops, it will receive a rare border to indicate that there is currently no better bow basetype available. Once "Bone Bows" (DropLevel = 24) become available because you moved to a higher zone, those will receive the border.

This is done for every Body Armour / Weapon basetype currently in the game.

## *Less* version filter

The goal of the original  `oftrta_map.filter` is the following:

> The "map version" displays significantly less normal and magic items while continuing to show recipe and high itemlevel items. I usually switch at mid tier maps.

So in this version, I fixed it a little bit to hide the low value items. Benefits is that your screen is not covered up by those item after a breach, incursion, etc.

- Hide low level/without quality/cheap gems
- Hide low value divination cards
- Hide chromatic orb recipes
- Hide low value rare items:
  + Regal recipes (low itemlevel)
  + Chaos recipes (low itemlevel)
  + Rares (low itemlevel)
  
  See [oftrta_map_less](https://github.com/noraj/OFTRTA-poe-filter/tree/oftrta_map_less) branch to get this custom filter.

## Other

For questions, F.A.Q., issues reporting, new ideas, changelog, pictures, in depth explanatrions, customization, credits, etc. go to the Path of Exile official [forum thread](http://www.pathofexile.com/forum/view-thread/1259059).

## Copyright / License

This work is licensed under the Creative Commons Attribution 3.0 Unported (CC BY 3.0) License.

To view a copy of this license, visit https://creativecommons.org/licenses/by/3.0/.
