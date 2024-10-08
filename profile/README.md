[![Discord](https://img.shields.io/discord/1279846081550618696?label=discord)](https://discord.gg/HzE9RgYPW5)

# Dofus Batteries Included (DBI)

## [DBI.Plugins](https://github.com/Dofus-Batteries-Included/DBI): Write plugins for Dofus Unity

Implements tools to write plugins for Dofus, and a few plugins.

### [Core](https://github.com/Dofus-Batteries-Included/DBI.Plugins/tree/main/src/Core) 

Implements common features for all plugins, in particular it adds the main DBI window to the game. The window allows to see and configure the plugins that have been loaded.

![DBI Core Window](https://raw.githubusercontent.com/Dofus-Batteries-Included/DBI.Plugins/main/img/general_tab.png)

### [TreasureSolver](https://github.com/Dofus-Batteries-Included/DBI.Plugins/tree/main/src/TreasureSolver)

Find the position of the next hint during treasure hunts and display it in the treasure hunt UI.

![Treasure Solver screenshot](https://raw.githubusercontent.com/Dofus-Batteries-Included/DBI.Plugins/main/img/treasure_hunt_widget.png)

## [DBI.Api](https://github.com/Dofus-Batteries-Included/DBI.Api): Share data collected by the plugins

Collection of APIs used by the DBI plugins. The main goal is to share data between the users of the plugins, e.g. treasure hunt clues.

### Data Center

Expose the data from [DDC](https://github.com/Dofus-Batteries-Included/DDC) (see below). 

### Treasure Solver

Solve treasure hunts. It is used by the [DBI.TreasureSolver](https://github.com/Dofus-Batteries-Included/DBI.Plugins/tree/main/src/TreasureSolver) plugin to
- solve treasure hunts
- record valid and invalid hints

The main goal is to collect data from all the players performing treasure hunts. The collected data can be exported through the [Export clues](https://treasuresolver-guf6a5ffd6amawh6.westeurope-01.azurewebsites.net/swagger/index.html#/Clues/Clues_ExportClues) endpoint.

# Dofus Data Center (DDC)
## [DDC](https://github.com/Dofus-Batteries-Included/DDC): Get data extracted from the game client

Exposes data extracted from the game client in [its Github Releases](https://github.com/Dofus-Batteries-Included/DDC/releases/tag/latest).