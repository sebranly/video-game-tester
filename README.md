# video-game-tester
This repository lists several indie video games I tested with pieces of advice to improve them. It doesn't focus on AAA games at all. For each game, it lists its pros and cons. It means that the feedback can be both positive and negative, but the overall goal of this repository is to be as constructive as possible in order to give every author ways to improve their projects.

These are my personal opinions about the games I test, some points will be objective (well-known accepted concepts about games like not having bugs) but most of them will be subjective. As a consequence, some points I mention can be criticized as well (for instance the fact that I prefer skill-based games rather than games based on luck).

## Disclaimer

I contact every author before reviewing their game (for instance the author might not want me to publish negative feedback on this public page and that's fine with me). You can still contact me here by creating an [issue](https://github.com/sebranly/video-game-tester/issues) or by using DM on Twitter ([@sebranly](https://twitter.com/sebranly)) and I'll do my best to solve the concern in a timely manner. For instance, if I mentioned a bug about your game and you fixed it, you can tag me so that I update the information available on this page. Also, I'd like readers to know that I'm aware that resources are limited (especially time and people) so I don't expect everything to be perfect in an indie game. This repository is trying to be as exhaustive as possible so that the authors can decide on their own where the priorities are for improving their projects.

## All Games

### Description

Rather than duplicating content in each game's section, this section lists common pieces of advice that are lengthy.

#### Open-source

Beginners should really force themselves to share their source code online by using code sharing tools like GitHub which is [free for public projects](https://github.com/pricing). A common mistake (that I made myself) is thinking that people might steal your awesome idea/pretend the project is theirs. Or thinking that the code is too messy to be shared publicly. However these concerns are far less important than having a whole community have a look at the code in order to give pieces of advice on how to improve it. People could even participate in the development of the project by developing new features if the author agrees. Later on, for a professional career in software development, having an open-source project that brought interest within a community (even if that's 10 people) is a real plus for the author because it shows they already have a foot into this field. At the same time, it can also help other people. For example, [BomberMario](https://github.com/sebranly/video-game-tester/blob/master/README.md#bombermario) was developed in C++/SFML and as a player who created similar 2D games in the past (Tetris, Sokoban, Mastermind, etc.), I'm interested in reading the source code because I have always used C/SDL for such projects (or C/PAlib on the Nintendo DS). Having feedback on the project itself is an awesome thing, but being able to have feedback on the source code (behind the scenes) is way better. Based on my personal experience, not making my projects open-source was a huge mistake, it made my (fairly little) projects die quickly.

#### Evolution

The game should bring more and more concepts as the player progresses. There are a lot of ways to achieve that, some of them are:
- introduce new enemies
- introduce new visual themes
- increase the difficulty
- introduce new power-ups

#### Level Editor

Whenever possible, it's always a good idea to implement a level editor so that players can create their own levels. It's an amazing plus if they can share them online (or through a copy/paste for less advanced projects that don't want to implement network interactions).

No matter what, every level editor should try to implement most of these things:
- include mouse controls
- include keyboard controls
- have textual explanations about the items being selected/used
- have textual explanations about keyboard controls, including how to test a level (which conditions need to be met to launch a level for example). For instance, if a level requires a starting point and an ending point to be playable, the level editor should mention it and mention what is respected by using :white_check_mark: and :x:
- offer simple controls. For instance, the player should be able to hold a key/mouse click and move to color a column/row of cells. A right click should be intuitive and delete the item.
- offer powerful tools, inspired by Paint. For instance, the player should be able to fill a region of cells, to draw a rectangle with a click/drag and drop, select a rectangular region of cells, copy and paste a region, perform symmetries, etc.

I think that the golden rule is to create the level editor at the very beginning of the project and then to use it for every single level. If such a process feels fastidious, it means that the players won't appreciate the level editor. Usually AAA games are built based on an internal level editor tool. Some of them even got released publicly, like Mario Maker for instance.

A real plus is to offer a progressive level editor based on the progress of the player within the game. For example, offer a selection of visual themes in the level editor once the player discovered them by playing the game.

## BomberMario

### Description

:bomb: Crossover between Bomberman and Mario as a 2D-game

- 👨‍💻 **Author:** Anthony Khelil ([@anthonykhelil](https://twitter.com/anthonykhelil/status/1043969866674438145))
- :calendar: **Release Date:** May 19, 2017
- TBD **Dates of the test:** End of December 2018
- TBD **Download Link:** https://www.anthony-khelil.fr/BomberMario/Download.php

### Pros

:white_check_mark: Nice things:

- :earth_americas: Support in English and French on the website
- :arrow_up_down: Full-screen mode
- :necktie: The overall project looks professional
- :black_circle: Nice transition effects in the menu
- TBD Several difficulty modes available in parallel at the beginning
- TBD Several platforms for the game (Windows and Mac)
- :notes: Music in the background and sound effects for auditive feedback depending on actions
- :runner: Smooth animations (the player and enemies don't move tile by tile but pixel by pixel)
- :chart_with_upwards_trend: New enemies appear in the game (ghosts that are more powerful because they can go through bricks)
- :busts_in_silhouette: Lots of enemies moving at the same time on the screen
- TBD Several levels are memorable (e.g. level 20 for the end of Easy Mode)
- TBD For multiplayer mode, each player has their own display for lives/scores that they picked in the settings (percentage or absolute)
- :arrow_upper_right: Diagonal moves are possible by holding two keys simultaneously (e.g. level 36)
- TBD A real difficult mode with some decent challenge (the player has to really pay attention to his stock of bombs otherwise they can be stuck somewhere with no bombs left nor lives and die quickly like in level 51)
- :pencil2: Good level design
- TBD Display of objects is smart by showing them individually then showing `x10` etc. when over 9 objects
- TBD Holding the `Space` key spawns bombs indefinitely without having to spam the `Space` key
- :game_die: Skill-based game rather than based on luck
- :zap: No performance drop at all (it never slows down)
- :bug: No bugs at all
- TBD Auto-save
- :bulb: Innovative gameplay
- TBD Really easy installation and doesn't take a lot of space
- TBD There is a level editor

### Cons

:x: Things that could be improved:

- :earth_americas: No English support within the game
- TBD The code is not open-source (see TBD)
- TBD The 3D mode is not well done at all, I didn't notice the change at first and went back to the settings to see if it was correctly saved. A real isometric view would look better and isn't that hard to implement (compared to real 3D).
- TBD Some issues about saving (as I didn't move the application within the `Applications` folder on Mac)
- TBD While in-game, it's not possible to pause/exit the game
- TBD I was a little bit surprised my bomb wouldn't make me die early in the game. Later on, when trying to complete difficult levels I understood such a decision
- :copyright: Video and audio files being used might be copyrighted and the source is not clearly mentioned (especially since it's Nintendo)
- :mouse: Mouse clicks don't work for selecting the menu or within the level editor
- TBD Animations are too limited (for instance the enemies don't have a sprite for up/down, they only have one for left/right, which looks odd when they move vertically)
- :hourglass_flowing_sand: Timer is missing, it could be an interesting addition to the gameplay/difficulty
- TBD The mouse is always displayed on screen (I'd expect not to see the cursor otherwise it's as annoying as watching a movie with the cursor appearing on top)
- TBD Pretty repetitive overall, there isn't a lot of evolutions happening through the game apart from the 3 different themes and the new type of enemies appearing (see TBD). For instance, it would have been amazing to get access to more power-ups like a star that makes the player invincible for a short period of time (like in Mario) so that the player can run through as many enemies as possible to kill them (like in Pac-Man). Another example would be to offer a special bomb (limited to 1) that has a longer radius of explosion (or maybe infinite). And another example could be a bomb that explodes bricks that cannot usually be destroyed. Playing in the same visual theme for 20 levels becomes a bit boring as well.
- TBD The level editor is really poor (see TBD)
- TBD Online game can be improved. For instance, it's misleading as it's not clear if this is competitive or co-operative. We were surprised by the fact the diamonds' changes (when player A picks one of them) were not reflected (player B still sees it, we understood why but it can be counter-intuitive as we can see each other's character). It felt like we were not really playing together because we didn't have a clear impact on each other except forcing one of the players to follow us in the next level. The online game wasn't really lagging in the way that my own character was running smoothly but the other player's character's progression was really slow to update (~3-4 seconds) despite playing in the same room. Also, the game froze (black screen) for the host after 4-5 levels and later on, creating/joining a new session was impossible for both of us despite killing/re-launching the app.
