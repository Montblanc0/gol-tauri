# Game of Life (Tauri Build)

My implementation of John Conway's [Game of Life](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life "Game of Life").

This is a simple [Tauri](https://tauri.studio/) build aimed at Windows machines. 

Original project made with [Angular CLI](https://github.com/angular/angular-cli "Angular CLI") version 13.2.6 (source TBA).

![Game of Life (Tauri Build)](https://i.ibb.co/XJ9gwyj/gol.jpg "Game of Life (Tauri Build)")

## Structure

- The topmost section just shows the title and a pair of gifs;
- The central area is a **40x40** interactive board that gets updated as the game progresses;
- the lowest part hosts controls and a generation counter:
 - "**Avvia/Pausa**" starts and pauses the game;
 - "**Random**" stops the game, resets the counter, clears the board and fills it with randomnly generated cells;
 - "**Clear**" stops the game and resets the counter;
 - "**Lento/Normale/Veloce**" (Slow, Normal, Fast) adjusts game speed (can also be used while the game is running).

### Download

See [Releases](https://github.com/Montblanc0/gol-tauri/releases) for downloads.

Only a binary file for Windows is provided in this repository (sources will be uploaded in another repository in the future).

### Instructions

This game follows the [original rules](https://en.wikipedia.org/wiki/Conway%27s_Game_of_Life#Rules) but also adds a "Pac-Man Effect" on every border.

You can draw your original generation by clicking on any box to toggle the alive/dead state while the board is clear and the game is not running.


Board interaction is **disabled** while the game is running.

Pause the game to edit the current generation and start it again to continue.

The game doesn't stop by itself when the board is clear or the game comes to a stall.