# pmr_item_tracker CHANGELOG

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [v0.4.0] - 2022-04-08
### ➕ Checks and logic for
- Chapter 5
  - Jade Jungle
  - Yoshi Village
  - Mt. Lavalava

### 🧹 Chores
- Adds a `CONTRIBUTING.md` file to help people new to contributing.
- Sets up repo Infrastructure as Code with `.github/settings.yml`.
- Sets up Semantic commit messages with `.github/semantic.yml`.
- Adds an [`.editorconfig` file](https://editorconfig.org/) to standardize formatting. (mostly helps Github Web UI users)

## [v0.3.0] - 2022-04-03
### ➕ Additional support for
- Partner abilities being always active.

### 🔄 Check updates
- Toad Town Tunnels
  - Chapter 5 warp check now toggles correct tracker flag.
- Koopa Village
  - Short name for shop items now displays correctly.
- Mt. Rugged
  - Adds logic for turning in letters to Parakarry for his partner quest.
- Shy Guy's Toybox
  - Color Box Puzzle now is in logic when you have the **Dictionary** and **Mystery Note**, without needing to set the tracker flag turning them in. (Russ T. in Toad Town - this may change if the color box puzzle's solution is randomized)
  - Checks for each station are indicated with the station's color.

### 🔄 Item updates
- Koopa Koot
  - Autograph items have been further optimized for ChatHUD: now can be toggled with `lauto` and `mauto`, for Luigi's and Merluvlee's autograph, respectively. (Randomizer has NYI Koopa Koot checks)

### 🔄 Layout updates
- Settings
  - Tracker settings are now contained in a popup - click the gear in the Star Spirits / Partners header.
- Condensed Star Spirits and partners into one header.

## [v0.2.0] - 2022-03-26
### ➕ Checks and logic for
- Chapter 4
  - Shy Guy's Toybox

### ➕ Support for
- Partner abilities being always active.

### 🔄 Check updates
- Boss battle check icons are now the Star Spirit card you would collect after the fight.

### 🌎 Map Updates
- Adds new map to allow separating Chapter 4 checks, as Toybox is incredibly dense.

## [v0.1.1] - 2022-03-24
### ➕ Checks and logic for
- Chapter 3
  - Forever Forest
  - Boo's Mansion
  - Gusty Gulch
  - Tubba Blubba's Castle

  ### ➕ Additional support for
- Shopsanity (as checks for regions are added)
- Coinsanity (as checks for regions are added)

## [v0.1.0] - 2022-03-22
### ➕ Added
- This CHANGELOG!
- Capturing items

### ➕ Checks and logic for
- Mt. Rugged
- Dry Dry Desert
- Dry Dry Outpost
- Dry Dry Ruins

### ➕ Support for
- Dry Dry Outpost starting location

### ➕ Additional support for
- Shopsanity (as checks for regions are added)
- Coinsanity (as checks for regions are added)

### ➕ Capturing items
- If you can see a check, but can't pick it up, this will allow you to mark the location with what the check contains.
- For example, the star piece in Toad Town across the water by the gate is a capturable check.
- Currently, only key items are capturable, other "priority" items will be added to the capture layout in the future. (maybe the hinted badges...? lmk!)

### 🔄 Item updates
- Added the Cookbook (was missing, whoops!)

### 🔄 Check updates
- Koopa Bros. Fortress: splits cracked walls in central hall to allow both to be captured
- Marked WIP or NYI settings with an X to indicate they do not function.
- Adds ability to exclude Star Piece Panels (not sure how I forgot this either)
- Panel checks now have a star piece icon to show their vanilla item.

### 🧹 Chores
- `images/flag/flagBlooper*.png`: removed images, tracker logic no longer relies on this flag
- `logic_helpers.lua`: added documentation comments

## [v0.0.7] - 2022-03-20
### ➕ Checks and logic for
- Shooting Star Summit
- Koopa Region
- Koopa Bros. Fortress

### ➕ Additional support for
- Shopsanity (as checks for regions are added)
- Coinsanity (as checks for regions are added)

### 🔧 Script fixes
- `can_access_star_haven()`: fixes reading incorrect setting
- `can_access_star_haven()`: returns earlier when configured for 0 spirits

## [v0.0.5] - 2022-03-19
### ➕ Added
- Broadcast view/ChatHUD
- Minimal, items only tracker
- More icons

### ➕ Checks and logic for
- Peach's Castle [WIP]
- Shooting Star Summit [WIP]
- Dojosanity

### ➕ Additional support for
- Configurable Star Spirit requirement
- Hidden block Watt requirement
- Shopsanity (as checks for regions are added)
- Coinsanity (as checks for regions are added)

### 🔄 Logic refactor
- More succinctly checks for Toad Town access

### 🧹 Chores
- All Files: newlines at EOF, because [a line isn't a line without \n](https://pubs.opengroup.org/onlinepubs/9699919799/basedefs/V1_chap03.html#tag_03_206)
- `location/world.json`: groups Toad Town checks by internal map ID

## [v0.0.3] - 2022-03-18
### ➕ Added
- A placeholder README
- A large map
- Initial layouts

### ➕ Initial data load of
- Star Spirits
- Partners
- Equipment
- Key Items
- Dungeon Keys
- Other Items
- Counters
- Settings

### ➕ Checks and logic for
- Goomba Region
- Toad Town
- Toad Town Tunnels

### ➕ Initial support for
- Starting location selection - Toad Town and Goomba Village

[v0.4.0]: https://github.com/IcySlurpee/pmr_map_tracker/compare/v0.3.0...v0.4.0
[v0.3.0]: https://github.com/IcySlurpee/pmr_map_tracker/compare/v0.2.0...v0.3.0
[v0.2.0]: https://github.com/IcySlurpee/pmr_map_tracker/compare/v0.1.1...v0.2.0
[v0.1.1]: https://github.com/IcySlurpee/pmr_map_tracker/compare/v0.1.0...v0.1.1
[v0.1.0]: https://github.com/IcySlurpee/pmr_map_tracker/compare/v0.0.7...v0.1.0
[v0.0.7]: https://github.com/IcySlurpee/pmr_map_tracker/compare/v0.0.5...v0.0.7
[v0.0.5]: https://github.com/IcySlurpee/pmr_map_tracker/compare/v0.0.3...v0.0.5
[v0.0.3]: https://github.com/IcySlurpee/pmr_map_tracker/tree/v0.0.3
