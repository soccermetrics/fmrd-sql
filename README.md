FMRD-SQL Version 1.3.5
======================

_This repository is no longer being supported.  Follow [this link](https://github.com/soccermetrics/marcotti) to the current Marcotti project._

This is the SQL implementation of the Football Match Result Database.
It currently operates on PostgreSQL and SQLite databases.

This implementation supports a data model for clubs participating in
league, knockout, or hybrid (league+knockout) competitions.  There 
are four categories under which the tables are classified:

* **Overview**: High-level data about the football competition
* **Personnel**: Participants and officials in the football match
* **Match**: High-level data about the match
* **Match Events**: The main events of the football match

The following tables are implemented:

Overview
--------

* Competitions
* Teams
* Venues
* VenueHistory

Personnel
---------

* Players
* PlayerHistory
* Managers
* Referees

Match
-----

* Matches
* Environments
* Lineups

Match Events
------------

* Goals
* Penalties
* Offenses
* Substitutions
* SwitchPositions
* PenaltyShootouts
* PenShootoutOpeners

The following validation tables are implemented:

Overview
--------

* FieldSurfaces
* Phases
* Groups
* Rounds
* KnockoutRounds
* Matchdays
* TimeZones
* WeatherConditions

Personnel
---------

* Confederations
* Countries
* FieldPositions
* FlankPositions
* Positions (composite)

Match
-----

* LeagueMatches
* GroupMatches
* KnockoutMatches
* HomeTeams
* AwayTeams
* HomeManagers
* AwayManagers
* KickoffWeather
* HalftimeWeather
* FulltimeWeather

Match Events
------------

* GoalEvents
* GoalStrikes
* PenaltyOutcomes
* Fouls
* Cards
* InSubstitutions
* OutSubstitutions

The following views are implemented:

Overview
--------

* TeamsList
* TimeZoneList
* VenueList
* VenueHistoryList

Personnel
---------

* PositionsList
* PlayersList
* PlayerHistoryList
* ManagersList
* RefereesList

Match
-----

* MatchList
* GroupMatchList
* LeagueMatchList
* KnockoutMatchList
* HomeTeamList
* AwayTeamsList
* KoWxList
* HtWxList
* FtWxList
* EnviroList
* LineupList

MatchEvents
-----------

* GoalsList
* OwnGoalsList
* PenaltiesList
* CautionsList
* ExpulsionsList
* SubsList
* InSubList
* OutSubList
* SwitchPosList
* ShootoutList
* ShootoutOpenersList

