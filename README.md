# Dofus Batteries Included (DBI)

## Write plugins for Dofus Unity

The [DBI](https://github.com/Dofus-Batteries-Included/DBI) project implements tools to write plugins for Dofus, and a few plugins.

### CorePlugin 

Implements common features for all plugins, in particular it adds the main DBI window to the game. The window allows to see and configure the plugins that have been loaded.

![DBI Core Window](https://raw.githubusercontent.com/Dofus-Batteries-Included/DBI/main/img/general_tab.png)

### [TreasureSolver](https://github.com/Dofus-Batteries-Included/DBI/tree/main/src/TreasureSolver)

Find the position of the next hint during treasure hunts and display it in the treasure hunt UI.

![Treasure Solver screenshot](https://raw.githubusercontent.com/Dofus-Batteries-Included/DBI/main/img/treasure_hunt_widget.png)

## Get data extracted from Dofus client

The [Dofus Data Center (DDC)](https://github.com/Dofus-Batteries-Included/DDC) project expose data extracted from the game client in [its Github Releases](https://github.com/Dofus-Batteries-Included/DDC/releases/tag/latest) and through [a REST API](https://ddc-gqaacvehagekdtcy.francecentral-01.azurewebsites.net/swagger).

## Treasure Solver
**WIP**

The [TreasureSolver](#) project provides a REST API to solve treasure hunts. It is used by the [DBI.TreasureSolver](https://github.com/Dofus-Batteries-Included/DBI/tree/main/src/TreasureSolver) plugin to
- solve treasure hunts
- record valid and invalid hints

The main goal is to collect data from all the players performing treasure hunts. The collected data can be exported through the [Export clues](#) endpoint. 