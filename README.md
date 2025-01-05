# idée de métriques importantes à prendre en compte pour la prédicition de victoire

# Infos importantes pour le dev 
ID de la Ligue 1 : 'idLeague': '4334', 'idSoccerXML': None, 'idAPIfootball': '6315'
ID de l'OL : 'idTeam': '133713', 'idESPN': '167', 'idAPIfootball': '80'

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

# Endpoint memo API

- */api/v1/json/3/eventsround.php?id=4334&r=16&s=2024-2025* : match in a specific round by league id/round/season. For league 1 the round correspond to the number of the day in the competition









# API à regarder 
https://www.football-data.org/
https://alexandrepa.github.io/footApi_website/?utm_source=chatgpt.com

# API testés mais pas ouf ou payantes
- https://www.api-football.com/ très bien mais donnée gratuites dispo uniquement entre 2020 et 2022
- https://www.sportmonks.com/ le plan gratuit n'inclu pas la ligue 1
- https://rapidapi.com/Creativesdev/api/free-api-live-football-data uniquement la saison 2024