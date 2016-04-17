# RankPoints
Set PurePerms Ranks Automatically using Rank Points

You MUST have PurePerms installed, the Ranks in RankPoints config.yml MUST all be existing PurePerms groups.

IMPORTANT:
The first rank MUST be the default PurePerms group, with points set to to zero.  Players with higher ranks will not be deranked.

RankPoints keeps track of points that are awarded to players using plugins such as VoteReward or TimeCommander which allow you to run commands (or on console).  PurePerms ranks are set automatically according to the config.

In-Game Commands:
/rankpoints - displays your own rank points
/rankpoints player - displays rank points for a player

Console or Plugin Commands:
rankpoints player points

Putting the following lines at the end of VoteReward

Commands:
  - "rankpoints {USERNAME} 1"

or running the command "rankpoints awzaw 1" on console, will add 1 point to the player awzaw's current rank points total, then check the config.yml which must be configured in this format, for example:

Ranks:
- Member
- Builder
- Admin
Points:
- 0
- 5
- 50

You MUST have PurePerms installed, the Ranks in RankPoints config.yml MUST all be existing PurePerms groups.

IMPORTANT:
The first rank MUST be the default PurePerms group, with points set to to zero.  Players with higher ranks will not be deranked.

TODO:
Permissions, allow settings points, custom success and help messages
