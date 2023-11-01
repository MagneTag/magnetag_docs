---
title: "Operating FEC Mode"
excerpt: "Operating your MagneTag system in full-service (FEC) mode"
toc: true
---

MagneTag's FEC mode is designed to be full-service. This means it works best when there's a dedicated person staffing the game,
adjusting the game is necessary. There are a lot more game play options in full-service mode than self-service (kiosk) mode.

## Players and Teams

In full-service mode, each player corresponds to a specific vest. We recommend adding labels to the physical vests that match the 
names displayed on screen for each vest -- this makes it a lot easier to get players organized into teams.

Players are organized into teams. Each team has a color, and each player on the team has a name. These names correspond to the armor
vests being used and aren't meant to be personalized with the real names of players.

There's a panel on the right side of the screen that displays match options, including buttons for adding and removing teams. The team
colors are always in the same order -- the first team is always red, the second team is always blue, etc.

The players on the team appear below the name of the team. There's also a list of "Unallocated Players". These are armor vests that
aren't currently in use for the upcoming match.

There are two ways to move a player between teams:
* Touch/click the name or icon for a player. They'll automatically move to the next team.
* Click the "Start Tag In" button. While in tag-in mode, hitting their armor vest with their sword will automatically move the player to
the next team. This can make it easier for players to choose their own teams.

There's also a "Clear All" that will remove all players from each team.

If a vest disconnects (for instance, if the battery dies or it goes out of range of the system), it'll automatically be moved to the list
of unallocated players.

## Match Settings

The panel on the right shows the different settings for the upcoming match. Some of these settings vary depending on the type of match.

### Match Type

There are currently two types of matches:
* **Combat** is the classic MagneTag game. Each team starts with a certain amount of health and loses health each time they're hit. The
last team with remaining health wins. This type of game can accommodate a wide range of players in any team configuration.
* **Time Tag** is an intense, countdown-based game. Each team starts with a certain amount of time on the clock. When they're hit,
their clock starts running down. When they hit their opponent, their clock stops running and their opponent's clock starts counting
down.

### Number of Games

MagneTag games are organized into matches, with the same players playing multiple games in a match. This specifies the number of games in a match. When a game is over, play automatically advances to the next game in the match.

### Play All Games

If there is more than one game in a match, this sets whether or not to play all the games after someone has won a majority of games. For instance, if there are three games in a match, and the red team wins the first two, this sets whether or not to play a third game.

### Audio Set

The audio set controls the audio and taunts used during the game. There are two modes:
* **Kids** provides family-friendly commentary during games.
* **Adult** taunts are still clean, but slightly harsher.

### Countdown Time

This sets the countdown time before each game in the match starts.

### Maximum Time

This sets the maximum length of a game. Normally a game ends when all teams but one are out of health, but this will cap the length of games.

### Double Hit Delay

The armor vests can be sensitive. If a hit is registered multiple times in a very short period of time, only one hit is registered. This sets the period of time during which only one hit will be counted.

### Combat Game Options

These options are specific to combat matches.

#### Starting Health

This is the health that each team starts with. With more players, we recommend increasing the starting health.

#### Health Per Hit

This is the health that a team loses every time a player is hit. We recommend keeping this at 1.

### Time Tag Options

These options are specific to time tag matches.

#### Starting Health

This is the amount of time each team starts with.

#### Regenerating Health Time

This is the amount of time a team gains back when their opponent's clock is active and their opponent is hit again. This allows a team to win back lost time.

#### Maximum Health Time

This is the maximum amount of time a team can have. If "Regenerating Health Time" is set to 0, this setting doesn't really matter.

## Notes

After several minutes of inactivity, the list of teams and the settings panel disappear from the screen. Just touch/click anywhere for them to reappear. The list of teams and settings panel can also be hidden by touching/clicking the "Hide Options" button.

For users with access to other controllers, there's a button for "Change Controller". This lets the operator switch to a different controller, like FEC/Kiosk mode or a tournament.

If running inside the MagneTag Shell, there's a "Shut Down" button with three options:
* **Log Off**: Closes the shell and logs out the current Windows user. This should only be used when needing to administer the PC.
* **Shut Down**: Closes the shell and turns off the PC.
* **Reboot**: Closes the shell and reboots the PC.

