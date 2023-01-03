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

### `importance` Rating

The importance rating specifies how important an event is within a league.
This value is optional and can be omitted, in which case it defaults to zero.

- `-1` a minor event, such as Festival of Combat Minor
- `0` a major event, such as a Festival of Combat Major
- `1` a very important event, such as Festival of Combat Finals

## `leagues.yml`

This file contains basic league information, such as organizers and hosts.
It also stores display information that describes what data about a tournament
is considered part of its name and what is merely metadata.

### `prestige` Rating

The prestige rating is a score which ranks the significance of a league.
This value is optional and can be omitted, in which case it defaults to zero.

- `-3..-1` weeklies, events with low player count, etc.
- `0` an ordinary community league or individual event
- `1` league with typically more skilled players
- `2` league with recurring events and highly skilled players (e.g. BttB)
- `3` league with recurring events, most skilled players, large price pools,
  tournaments of high production value, etc. (currently just Festival of Combat)

## `scoreboards.yml`

This file contains basic scoreboard information, such as names and platforms.