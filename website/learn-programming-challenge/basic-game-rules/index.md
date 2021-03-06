---
layout: doc_page
title: Basic Game Rules
toc: false
description: Get an introduction to the rules of the game to win the Halite AI Programming Challenge.
sort_key: 0
---
Here is a quick overview of the rules of Halite II. If you want to get into the nitty-gritty, check out our [Game Rules Deep Dive](game-rules-deep-dive).

## Map at Game Start
Halite II is played on 2D map, which is set up as a continuos Cartesian plane (think of it has having x/y axes). The map is like a virtual game board, and does not wrap, meaning that game pieces can fall off the edges of the board, they don't appear on the opposite side like an old school arcade game.

<div class="static-container text-center">
    <img style="width: 100%; height: auto;" src="/assets/images/tutorial-images/map-at-game-start.png" alt="Halite Game Board at Start of Game">
</div>

<br>Maps are randomly and symmetrically generated, and consist of a number of planets at start. At the start, all planets are neutral and players own none of them. The sizes and locations of planets also varies map to map.

## Starting a game
Two or four players compete in a match. 
At the start of the game, each player will have 3 ships on the map.

## Players each have a fleet of ships

As mentioned, players have 3 ships at the start of the game. You move ships around the map using three commands.
1. Ships can be commanded to move with a given angle and a velocity.
2. Ships can also “dock” to  a planet.
3. Ships can “undock” from a planet.

This is a ship in flight:

<div class="static-container text-center">
    <img style="width: 40%; height: auto;" src="/assets/images/tutorial-images/ship-in-flight.png" alt="Halite ship in flight">
</div>

<br>The circle around the ship is its aura, which is uses to measure the offensive/defensive reach of the ship. Ships may be destroyed through battle or collision with each other and planets, and they have an initial health and lose health as they battle.

<div class="static-container text-center">
    <img style="width: 40%; height: auto;" src="/assets/images/tutorial-images/ships-in-combat.jpeg" alt="Halite ships in combat">
</div>

Ships collide when they try to occupy the same location on the map.

## Planets are for producing new ships

<br>Ships can 'dock' on planets to mine Halite and produce more ships. This is a ship docked to a planet:

<div class="static-container text-center">
    <img style="width: 40%; height: auto;" src="/assets/images/tutorial-images/final-composite.png" alt="Halite ship docked on a planet">
</div>

<br>Each player can dock ships simultaneously on multiple planets, but only ships from one player can dock on a particular planet at a time. The number of ships that can be docked to a planet is determined by the planet size.

When a ship docks on a planet, the planet produces ships for the docked player. Planets produce at a constant rate per ship with no limit to ship production.

Planets can be destroyed through ship collisions. Boom.

<div class="static-container text-center">
    <img style="width: 40%; height: auto;" src="/assets/images/tutorial-images/planet-exploding.png" alt="Halite planet explosion">
</div>

## Win conditions
1. A player is the sole survivor.
2. A player occupies all planets. This means they must have a ship fully docked to all remaining planets; a ship that is in the process of docking does not count.
3. If time runs out and neither of these conditions are met, tiebreaker rules apply:
    - First we check to see which surviving team has produced the most ships.
    - If still a tie, then we check to see which team has done the most battle damage (destroying ships with other ships through attacks or collision).
    - If still a tie, a random winner will be chosen, but this outcome has a very low probability of occurring given the other winning conditions.

## Note on game rules changes
The Two Sigma and Halite team reserves the right to make changes on game rules during the course of the game. We promise we won't do this without a very good reason that improves the competition and the fun of the game, and we will try to make any changes as backwards compatible as possible.

