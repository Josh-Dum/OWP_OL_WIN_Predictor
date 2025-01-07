# idée de métriques importantes à prendre en compte pour la prédicition de victoire

# Infos importantes pour le dev 

## ligue 1 
ID de la Ligue 1 : 'idLeague': '4334', 'idSoccerXML': None, 'idAPIfootball': '6315'
ID de l'OL : 'idTeam': '133713', 'idESPN': '167', 'idAPIfootball': '80'
le round correspond au numéro de journée de ligue 1

## Coupe de France
ID de la Coupe de France : "idLeague": "4484", "idAPIfootball": "6844"

Differents values of int round : 
- 200 : final
- 150 : Semi-Final
- 125 : Quarter-Final
- 16 : 8e de finale
- 32 : 16e de finale
- 64 : 32 ème de finale

OL does not play before 32 final

## Champions league
ID of Champions league : "idLeague": "4480", "idSoccerXML": null, "idAPIfootball": "6281"

Differents values of int round : 
- 200 : final
- 150 : Semi-Final
- 125 : Quarter-Final
- 16 : 8e de finale
- 1 : Group stage - Day 1
- 2 : Group stage - Day 2
- 3 : Group stage - Day 3
- 4 : Group stage - Day 4
- 5 : Group stage - Day 5
- 6 : Group stage - Day 6
- 7 : Group stage - Day 7
- 8 : Group stage - Day 8




# API choisie
https://www.thesportsdb.com/free_sports_api

# Explication des champs utilisés pour les donées 

- idEvent : id d'un match de foot dans l'API 
- strEvent : String qui contient le nom de l'event, dans mon cas le format sera comme ça "Nice vs Lille"
- strSeason : String qui contient les années de début et de fin de la saison de foot sous ce format : "2023-2024"
- intHomeScore : entier qui représente le nombre de but marquée par l'équipe qui joue à domicile
- intAwayScore : entier qui représente le nombre de but marquée par l'équipe qui joue à l'extèrieur
- idHomeTeam : id de la team qui joue à domicile dans l'API
- idAwayTeam : id de la team qui joue à l'extèrieur dans l'API

need to add : 
round for leagues

# Endpoint memo API

- */api/v1/json/3/eventsround.php?id=4334&r=16&s=2024-2025* : match in a specific round by league id/round/season. For league 1 the round correspond to the number of the day in the competition
- */api/v1/json/3/search_all_leagues.php?c=France&s=Soccer* : List all Leagues in France for football









# API à regarder 
https://www.football-data.org/
https://alexandrepa.github.io/footApi_website/?utm_source=chatgpt.com

# API testés mais pas ouf ou payantes
- https://www.api-football.com/ très bien mais donnée gratuites dispo uniquement entre 2020 et 2022
- https://www.sportmonks.com/ le plan gratuit n'inclu pas la ligue 1
- https://rapidapi.com/Creativesdev/api/free-api-live-football-data uniquement la saison 2024