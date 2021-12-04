
This is a non exhaustive list of endpoints from the ESPN hidden NFL API
* ! * See the player_id.csv and team_id.csv For lists of active player Id's and team Id's * ! *


Scores for current week
    http://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard


Scores by week (current season)
    http://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard?seasontype={SeasonType}&week={Week #}
    -Season types are:
        -1: Preseason
            weeks 1-4 (HOF game is week=1)
        -2: Regular Season
            weeks 1-18
        -3: Post Season
            Week #'s
            -#1 = Wild Card Round
            -#2 = Divisional Round
            -#3 = Conference Championships
            -#4 = Super Bowl


One Game 
    http://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard/{gameId}
        -ex: (Dallas at New Orleans) http://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard/401326509


Latest News:
    http://site.api.espn.com/apis/site/v2/sports/football/nfl/news


One Article:
    http://now.core.api.espn.com/v1/sports/news/{articleId}
        -ex: (article) http://now.core.api.espn.com/v1/sports/news/32765116


All teams:
    https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams?limit=32


One Team: 
    https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/{teamId OR team abbreviation} 
        -ex: (Cleveland Browns) https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/cle               
        -ex: (Cleveland Browns) https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/5                


One Team Roster 
    https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/{teamI OR team abbreviation}/roster
        -ex: (Cleveland Browns Roster) https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/cle/roster        
        -ex: (Cleveland Browns Roster) https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/5/roster          


Full team stats 
    https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/{teamI OR team abbreviation}/statistics
        -ex: (Cleveland Browns statistics) https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/cle/statistics        
        -ex: (Cleveland Browns statistics) https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/5/statistics  


One team full schedule
    https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/{teamI OR team abbreviation}/schedule
        -ex: (Cleveland Browns schedule) https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/cle/schedule        
        -ex: (Cleveland Browns schedule) https://site.api.espn.com/apis/site/v2/sports/football/nfl/teams/5/schedule  


One Player
    https://site.web.api.espn.com/apis/common/v3/sports/football/nfl/athletes/{playerId}
        -ex: (Nick Chubb) https://site.web.api.espn.com/apis/common/v3/sports/football/nfl/athletes/3128720  


One player's full stats for each year played (includes career totals)
     https://site.web.api.espn.com/apis/common/v3/sports/football/nfl/athletes/{playerId}/stats
        -ex: (Nick Chubb Full stats) https://site.web.api.espn.com/apis/common/v3/sports/football/nfl/athletes/3128720/stats  


Standings current season
    https://site.api.espn.com/apis/v2/sports/football/nfl/standings


Standings specific seaon  
    https://site.api.espn.com/apis/v2/sports/football/nfl/standings?season={year}
        ex: https://site.api.espn.com/apis/v2/sports/football/nfl/standings?season=2019 


Photos
    -Player headshot
        https://a.espncdn.com/i/headshots/nfl/players/full/{playerId}.png
            -ex: (Nick Chubb headshot) https://a.espncdn.com/i/headshots/nfl/players/full/3128720.png

    -Team Logo (500px)
        https://a.espncdn.com/i/teamlogos/nfl/500/{team abbreviation}.png
            -ex: (Browns Logo) https://a.espncdn.com/i/teamlogos/nfl/500/cle.png
