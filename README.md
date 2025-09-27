# XiangqiMobile
Mobile-first xiangqi web app

1 server will need to host the web app for the UI and game
for the player to play on.  This will be the static server
hosted either locally with Node or something like Itch.io.

1 server will need to host the game.  This doesn't show any
game content and the players can't interact with it directly
but their game client will communicate with it to send and
receive info about the game state.  This cannot be on Itch.io.

In the meantime, for testing, I'll use Node to host the game
content locally ("serve ." in the directory of the exported
game files) and Nakama to host the game server locally
(docker-compose up in directory with docker-compose.yml)
