# Ball-Bouncing-Game

<h2> <b> PROBLEM STATEMENT </b> </h2>

  The goal of the program is to create a ball bouncing game, including a slider and a ball. The game can be played in
  Two-Player mode using 2 sliders as well. The game is over when a player fails to hit the ball with his slider in time,
  and lets the ball ‘miss’.

<h2> <b> PROBLEM DEFINITION </b> </h2>

1. Single Player Mode – How long can the player manage to hit the ball?
2. 2 Player Mode – 2 players play at the same time, controlling different sliders. Whoever misses the ball
loses.
3. Game gets progressively difficult – Speed of ball increases automatically, Size of slider continually
reduce
4. Pause Game Feature.
5. Scoring System
6. Recording top 3 scores of all time
7. Settings – User can optimize play area size, and slider length
8. Can be played multiple times in the same runtime- User can return to main menu after game over to start
new game, view scores etc.

<h2> <b> OVERVIEW / BACKGROUND DETAILS </b> </h2>

  The goal of the program is to create a ball bouncing game, including a slider and a ball. The game can be played in
  both Two-Player mode(with 2 sliders) and Single-Player mode. In 1P mode the game is over when a player fails to
  hit the ball with his slider in time, and lets the ball ‘miss’. The number of times the user hits the ball is his score. In
  2P mode, when a player misses the ball, the other player wins.

  The top 3 highscores of all time are recorded in 1P mode. The highscores can be reset if the user wants to. Settings
  can be changed to optimize game according to user’s wants (change play area size, slider size). The game gets
  progressively difficult, as the ball speed increases and the length of slider continually decrease, after user has hit a
  certain score.

  The dynamic nature of the ball is implemented using a matrix which stores the present state of the ball and the play
  area (excluding the two sliders). The matrix changes continuously after fixed intervals of time, according to the
  present locus of the ball. Each state of the matrix is shown after that fixed interval (using a basic chain of OUTPUT
  -> wait-> UPDATE NEW POSITION-> CLEAR SCREEN-> OUTPUT) giving the feel of dynamic movement of the ball.

  The locus of the ball is updated using 4 chief parameters. First two (x,y) being the current locus of the ball with
  respect to the row and column position in the play-area matrix. The other two (xdir, ydir) stores the direction of the
  ball along the row and column. For example if the ball is moving up, then its locus along rows is continuously
  decreasing. So ydir(direction of rows) will be -1. Similarly, when ball is going downward, ydir=+1. When ball goes
  left, xdir=-1 (it is going towards column=0), and when it goes right, xdir=+1.
  The value of (x, y) are changed after every interval of time by (x+xdir,y+ydir)

  When the ball hits a wall, the values of xdir and ydir are changed accordingly.

  <h2> <b> DISCUSSIONS </b> </h2>
  
  The program automatically increases game speed and shortens the slider length to make it difficult and challenging
  for players. The scoring system is simple and uses simple file handling methods to store highscores. The game can
  be optimized as the user wants from the settings tab. In 2 player mode, the players can play on the same keyboard
  with each player controlling a different slider.     

<h2> <b> IMPROVEMENTS </b> </h2>
  
  There can however be many improvements to the game. Since it is a game, the possibilities of expanding are
  tremendous. While we consider the program to be more than just a prototype, some of the features like Graphics, Multiplayer Online / LAN, Tournament Mode, 4-player Mode, Obstacles in the play area or Power-Ups can be added to make the experience better.

<h3><a id="user-content-liked-this-project-did-it-help-you-leave-a-star-fork-and-share-the-love" class="anchor" aria-hidden="true" href="#liked-this-project-did-it-help-you-leave-a-star-fork-and-share-the-love"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"></path></svg></a>Liked this project? Did it help you? Leave a <a href="https://github.com/EshaNandy94/Ball-Bouncing-Game/stargazers">star</a>, <a href="https://github.com/EshaNandy94/Ball-Bouncing-Game/network/members">fork</a> and share the love!</h3>
