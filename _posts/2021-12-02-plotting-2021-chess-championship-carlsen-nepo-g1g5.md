---
layout: post
title: The Draws Continue in Games 1-5 of the 2021 World Chess Championship
date: 2021-12-02 20:21:55 -0300 
use-site-title: true
comments: true
archive: true
subscribe: true
image: /img/wcc_logo_2021.png
tags:
- Chess
- Win expectancy
- R
---

Running back to Game 10 of the <a href = "https://en.wikipedia.org/wiki/World_Chess_Championship_2016" target = "_blank">2016 World Chess Championship</a>, there have now been 19 straight draws in the classical portions of these championship matches. The five most recent entries in this draw-streak have come from the <a href = "https://en.wikipedia.org/wiki/World_Chess_Championship_2021" target = "_blank">2021 Championship</a> in which World No. 1, Magnus Carlsen, is battling World No. 5 Ian Nepomniachtchi ("Nepo"). Carlsen has been champion since 2013 when he <a href = "https://en.wikipedia.org/wiki/World_Chess_Championship_2013" target = "_blank">defeated Viswanathan Anand</a>. He has defended his title three times: in <a href = "https://en.wikipedia.org/wiki/World_Chess_Championship_2014" target = "_blank">2014</a> against Anand, in 2016 against Sergey Karjakin, and in <a href = "https://en.wikipedia.org/wiki/World_Chess_Championship_2018" target = "_blank">2018</a> against Fabiano Caruana; the match that contributed 12 draws to the ongoing 19-draw streak.

As I did for <a href = "https://www.cteeter.ca/blog/2018-11-20-plotting-2018-chess-championship-carlsen-caruana/" target = "_blank">the</a> <a href = "https://www.cteeter.ca/blog/2018-11-26-plotting-2018-chess-championship-carlsen-caruana-g9to12/" target = "_blank">games</a> and <a href = "https://www.cteeter.ca/blog/2018-11-28-plotting-2018-chess-championship-carlsen-caruana-tiebreaks/" target = "_blank">tiebreaks</a> of the 2018 match, I have been following <a href = "https://www.chess.com/events/2021-fide-world-chess-championship" target = "_blank">Chess.com's coverage of the games</a> and noodling around on the <i>Analysis Tool</i> at <a href = "https://lichess.org/analysis" target = "_blank">Lichess.org</a> (which runs the <a href = "https://en.wikipedia.org/wiki/Stockfish_%28chess%29" target = "_blank">Stockfish</a> simulation engine) in order to evaluate which player has an advantage (if any) after each move. 

The advantage a player has is measured in <i>Pawn Advantage Units</i>. The simulation engine takes a given position and projects play forward for some number of moves, anticipating what the board will look like if the players play optimally. A pawn advantage unit of +1.0 indicates the player with White pieces is (theoretically) up a pawn, meaning that player has (or could have, with the right sequence of moves) one more pawn than the player with the Black pieces. That might not sound like a lot, but at the level of the players in these championships, having even that small of an advantage often results in victory. Being +3.0 represents a lead of a <a href = "https://en.wikipedia.org/wiki/Chess_piece_relative_value" target = "_blank">minor piece</a> (Bishop, Knight), +5.0 is up a rook, and so on.

Here is how the first three games of the 2021 match have progressed in pawn advantage units:

<center><img src="/img/posts/20211202/wcc2021_G1toG3.png" style="width:98%"></center>

Pawn advantage units are on the y-axis (from -5.0 to +5.0), converted to be displayed with reference to the player. Moves are on the x-axis, with the key time control moments indicated. The players each get 120 minutes for their first 40 moves. After they complete 40 moves they get 60 minutes added to their clock. After they reach 60 moves, another 15 minutes is added, with an increment of 30 seconds per move starting on move 61. As you can see in the figure above, none of the games have reached move 60, and neither player has managed to get much of an advantage. In Game 2, Nepo had something going (slightly more than a pawn advantage around move 20) but his advantage was quickly extinguished by a combination of Magnus' strong defense and his own reluctance to play aggressively.

After Game 3 the players had a rest day, but in Game 4 things picked up where they left off in Game 3:

<center><img src="/img/posts/20211202/wcc2021_G4andG5.png" style="width:98%"></center>

In all, 436 moves have been made across the five games, only six of those have resulted in one player having an advantage greater than 1.0. These guys are just too good when they have this much time to consider their moves. They have prepared so deeply using the chess engines that are used to evaluate the positions, that they are essentially representations of the chess engines. Their accuracy is incredible. 

The folks at Lichess explored <a href = "https://lichess.org/blog/YafSBxEAACIAr0ZA/exact-exacting-who-is-the-most-accurate-world-champion" target = "_blank">how accurate Magnus and Nepo have been in this match</a>. They compared their moves to what the Stockfish engine's suggested moves and found that this year's match has included the most accurate play in the history of Chess Championships:

<center><img src="/img/posts/20211202/lichess_wcc_accuracy.png" style="width:92%"></center>

That figure shows <i>average centipawn loss</i> on the y-axis, which is essentially the difference between a player's move and the engine's move in pawn advantage units; lower is more accurate. Things have been getting more and more accurate over time.

The analysis from Lichess is important. It is often the case that a drawn game is viewed as boring. We want to see someone win. But perfect play will result in a draw and Magnus and Nepo are playing as close to perfect as has ever been seen in a World Championship. The precision makes for tense moments, as the level of play is so high and any deviation could spell trouble for one of the players. But thus far they haven't made any clear mistakes, and as Nepo suggested during one of the press conferences, it will take a mistake for someone to break through and win.

Game 6 goes tomorrow, after today's rest day. Carlsen gets his third chance with the White pieces maybe he can force an advantage with them. I will be tracking the remaining games.