# Souls Player Data

This database in the form of yml files contains neatly organized information
about DS3/Elden Ring players and past tournaments.

## `players.yml`

This file contains player information, such as Discord ids and other social
media connections, titles, noteworthy facts, etc.

The `score` field of a player refers to an entry in `scoreboards.yml`.

## `events.yml`.

This file contains event information, such as date, league, platform, region,
and winners up to top 4, or top 3 if the third place is shared.

The names of `winners` refer to players in `players.yml`.
The `league` refers to an entry in `leagues.yml`.

## `leagues.yml`

This file contains basic league information, such as organizers and hosts.
It also stores display information that describes what data about a tournament
is considered part of its name and what is merely metadata.

## `scoreboards.yml`

This file contains basic scoreboard information, such as names and platforms.