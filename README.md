# video-game-tester
This repository lists several indie video games I tested with pieces of advice to improve them. It doesn't focus on AAA games at all. For each game, it lists its pros and cons. It means that the feedback can be both positive and negative, but the overall goal of this repository is to be as constructive as possible in order to give every author ways to improve their projects.

These are my personal opinions about the games I test, some points will be objective (well-known accepted concepts about games like not having bugs) but most of them will be subjective. As a consequence, some points I mention can be criticized as well (for instance the fact that I prefer skill-based games rather than games based on luck).

## Disclaimer

I contact every author before reviewing their game (for instance the author might not want me to publish negative feedback on this public page and that's fine with me). You can still contact me here by creating an [issue](https://github.com/sebranly/video-game-tester/issues) or by using DM on Twitter ([@sebranly](https://twitter.com/sebranly)) and I'll do my best to solve the concern in a timely manner. For instance, if I mentioned a bug about your game and you fixed it, you can tag me so that I update the information available on this page. Also, I'd like readers to know that I'm aware that resources are limited (especially time and people) so I don't expect everything to be perfect in an indie game. This is basically my take on the games I tested. This repository is trying to be as exhaustive as possible so that the authors can decide on their own where the priorities are for improving their projects.

## To-Do List

This lists the general tasks I should complete to improve this repository

- Have French translations to reach a wider audience
- Push further the testing for the games by following their `Disclaimer` sections

## Summary

- [BomberMario](https://github.com/sebranly/video-game-tester/blob/master/README.md#bombermario)
- [Super Pokemon Run](https://github.com/sebranly/video-game-tester/blob/master/README.md#super-pokemon-run)

## All Games

### Description

Rather than duplicating content in each game's section, this section lists common pieces of advice that are lengthy.

#### Open-source

Beginners should really force themselves to share their source code online by using code sharing tools like GitHub which is [free for public projects](https://github.com/pricing). A common mistake (that I made myself) is thinking that people might steal your awesome idea/pretend the project is theirs. Or thinking that the code is too messy to be shared publicly. However these concerns are far less important than having a whole community have a look at the code in order to give pieces of advice on how to improve it. People could even participate in the development of the project by developing new features if the author agrees. Later on, for a professional career in software development, having an open-source project that brought interest within a community (even if that's 10 people) is a real plus for the author because it shows they already have a foot into this field. At the same time, it can also help other people. For example, [BomberMario](https://github.com/sebranly/video-game-tester/blob/master/README.md#bombermario) was developed in C++/SFML and as a player who created similar 2D games in the past (Tetris, Sokoban, Mastermind, etc.), I'm interested in reading the source code because I have always used C/SDL for such projects (or C/PAlib on the Nintendo DS). Having feedback on the project itself is an awesome thing, but being able to have feedback on the source code (behind the scenes) is way better. Based on my personal experience, not making my projects open-source was a huge mistake, it made my (fairly little) projects die quickly.

#### Evolution

The game should bring more and more concepts as the player progresses. There are a lot of ways to achieve that, some of them are:
- introduce new enemies
- introduce new visual themes (this is really easy to implement with a tileset, yet it completely changes the way the player perceives the game)
- increase the difficulty
- introduce new power-ups
- introduce an endless mode that relies on [procedural generation](https://en.wikipedia.org/wiki/Procedural_generation) to offer an infinity of new levels
- promote retention by having scoring systems so that the player wants to improve their own score

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

A real plus is to offer a progressive level editor that contains more and more features/items based on the progress of the player within the game. For example, offer a selection of visual themes in the level editor once the player discovered them by playing the game.

### All Games Table

|Features/Games|BM|SPR|
|-|-|-|
|:rewind: While in-game, the player can pause/exit the game|:x:|:white_check_mark:|
|:pencil2: Interesting level design|:white_check_mark:|:white_check_mark:|
|:notes: Music in the background and sound effects for auditive feedback depending on actions|:white_check_mark:|:white_check_mark:|
|:bar_chart: Good gameplay evolution (see [this section](https://github.com/sebranly/video-game-tester/blob/master/README.md#evolution))|:x:|:white_check_mark:|
|:earth_americas: Support in English and French on the website|:white_check_mark:|:white_check_mark:|
|:earth_americas: French and English support within the game|:x:|:white_check_mark:|
|:octocat: The code is open-source (see [this section](https://github.com/sebranly/video-game-tester/blob/master/README.md#open-source))|:x:|:x:|
|:arrow_up_down: Full-screen mode|:white_check_mark:|:white_check_mark:|
|:necktie: The overall project looks professional|:white_check_mark:|:x:|
|:black_circle: Nice transition effects in the menu|:white_check_mark:|:white_check_mark:|
|:cd: Several platforms for the game (Windows and Mac)|:white_check_mark:|:white_check_mark:|
|:runner: Smooth animations (the player and enemies don't move tile by tile but pixel by pixel)|:white_check_mark:|:white_check_mark:|
|:chart_with_upwards_trend: New enemies appear in the game|:white_check_mark:|:white_check_mark:|
|:busts_in_silhouette: Lots of enemies moving at the same time on the screen|:white_check_mark:|:white_check_mark:|
|:dart: Skill-based game rather than based on luck|:white_check_mark:|:white_check_mark:|
|:zap: No performance drop at all (it never slows down)|:white_check_mark:|:x:|
|:bug: No bugs at all|:white_check_mark:|:x:|
|:floppy_disk: Auto-save|:white_check_mark:|:white_check_mark:|
|:bulb: Innovative gameplay|:white_check_mark:|:white_check_mark:|
|:balloon: Really easy installation and doesn't take a lot of space|:white_check_mark:|:white_check_mark:|
|:recycle: There are special tokens/coins to obtain per level in order to encourage the player to retry the same level|:white_check_mark:|:white_check_mark:|
|:copyright: Video and audio files being used belong to the author or the source is clearly mentioned (especially since it's Nintendo)|:x:|:x:|
|:mouse: Mouse clicks don't work for selecting the menu or within the level editor|:x:|:x:|
|:mouse: The mouse is properly hidden from the screen (I'd expect not to see the cursor otherwise it's as annoying as watching a movie with the cursor appearing on top)|:x:|:x:|
|:gem: The menu should show hints about the progression of the player. For instance when on the menu, I'd like `Adventure` to have an icon or a progress bar indicating how far I completed the overall game.|:x:|:x:|

Caption:
- Games
  - BM stands for [BomberMario](https://github.com/sebranly/video-game-tester/blob/master/README.md#bombermario)
  - SPR stands for [Super Pokemon Run](https://github.com/sebranly/video-game-tester/blob/master/README.md#super-pokemon-run)
- Features
  - :x: means the game doesn't have the feature but it should have it
  - :white_check_mark: means the game has the feature
  - Nothing means that the game doesn't have the feature but it doesn't matter because it's not expected

## BomberMario

### Description

:bomb: Crossover between Bomberman and Mario as a 2D-game

- 👨‍💻 **Author:** Anthony Khelil ([@anthonykhelil](https://twitter.com/anthonykhelil/status/1043969866674438145))
- :calendar: **Release Date:** May 19, 2017
- :mag: **Dates of the test:** End of December 2018 (version 1.2) on Mac
- :arrow_down: **Download Link:** https://www.anthony-khelil.fr/BomberMario/Download.php

### Disclaimer

I didn't finish the game up to 100%. For instance, I hardly tested the online mode, hardly tested the endless solo mode, and although I completed all adventure levels, I didn't try to get all 4 tokens for each of them. If some points below are incorrect please let me know. I fully read the [blog article](https://www.anthony-khelil.com/Article.php?ID=2&Language=English).

**For all pros and cons, don't forget to also check out the [All Games Table](https://github.com/sebranly/video-game-tester/blob/master/README.md#all-games-table)**

### Pros

:white_check_mark: Nice things:

- :performing_arts: Several difficulty modes available in parallel at the beginning
- :crystal_ball: Several levels are memorable (e.g. level 20 for the end of Easy Mode)
- :restroom: For multiplayer mode, each player has their own display for lives/scores that they picked in the settings (percentage or absolute)
- :arrow_upper_right: Diagonal moves are possible by holding two keys simultaneously (e.g. level 36)
- :heart_decoration: A real difficult mode with some decent challenge (the player has to really pay attention to his stock of bombs otherwise they can be stuck somewhere with no bombs left nor lives and die quickly like in level 51)
- :keycap_ten: Display of objects is smart by showing them individually then showing `x10` etc. when over 9 objects
- :arrows_counterclockwise: Holding the `Space` key spawns bombs indefinitely without having to spam the `Space` key
- :triangular_ruler: There is a level editor

### Cons

:x: Things that could be improved:

- :game_die: The 3D mode is not well done at all, I didn't notice the change at first and went back to the settings to see if it was correctly saved. A real isometric view would look better and isn't that hard to implement (compared to real 3D).
- :floppy_disk: Some issues about saving (as I didn't move the application within the `Applications` folder on Mac)
- :skull: I was a little bit surprised my bomb wouldn't make me die early in the game. Later on, when trying to complete difficult levels I understood such a decision
- :left_right_arrow: Animations are too limited (for instance the enemies don't have a sprite for up/down, they only have one for left/right, which looks odd when they move vertically)
- :hourglass_flowing_sand: Timer is missing, it could be an interesting addition to the gameplay/difficulty
- :repeat_one: Pretty repetitive overall, there isn't a lot of evolutions happening through the game apart from the 3 different themes and the new type of enemies appearing (see [this section](https://github.com/sebranly/video-game-tester/blob/master/README.md#evolution)). For instance, it would have been amazing to get access to more power-ups like a star that makes the player invincible for a short period of time (like in Mario) so that the player can run through as many enemies as possible to kill them (like in Pac-Man). Another example would be to offer a special bomb (limited to 1) that has a longer radius of explosion (or maybe infinite). And another example could be a bomb that explodes bricks that cannot usually be destroyed. Playing in the same visual theme for 20 levels becomes a bit boring as well.
- :triangular_ruler: The level editor is really poor (see [this section](https://github.com/sebranly/video-game-tester/blob/master/README.md#level-editor))
- :signal_strength: Online game can be improved. For instance, it's misleading as it's not clear if this is competitive or co-operative. We were surprised by the fact the diamonds' changes (when player A picks one of them) were not reflected (player B still sees it, we understood why but it can be counter-intuitive as we can see each other's character). It felt like we were not really playing together because we didn't have a clear impact on each other except forcing one of the players to follow us in the next level. The online game wasn't really lagging in the way that my own character was running smoothly but the other player's character's progression was really slow to update (~3-4 seconds) despite playing in the same room. Also, the game froze (black screen) for the host after 4-5 levels and later on, creating/joining a new session was impossible for both of us despite killing/re-launching the app.
- :globe_with_meridians: No mini-map is displayed. That might have been a choice not to make the gameplay too easy. I think in that case, the mini-map could have been a special item that is hidden that the player has to pick in order to have a global overview of the map/ennemies' position as a reward
- :zzz: There is no change of music or clear change of display when the player is about to die. It's hard to focus on the enemies moving quickly/the health bar. An additional video/audio indicator when there is only one life left could be good.
- :hocho: A hardcode mode could be good. It could be a mode with a maximum of 3 lives for instance, or a mode that doesn't display any bomb/lives indicator on screen. We can also imagine a level in which enemies keep spawning (with a maximal threshold) until the "generator of enemies" is destroyed with a bomb by the player. Or it could be a level in which there are no safe zones (i.e. the enemies can move everywhere the player can move).
- :neutral_face: Difficult levels become less interesting after a while once the player realizes that the best technique is to wait on a bomb spawner and hold `Space` key to kill enemies for 2-3 minutes before doing any move. One easy solution would be to include a 1-by-1 safe spot with a bomb spawner on it so that the player can target 4 cells at the same time (I think the maximum of targetable cells I've seen was 3 (the 4th one was a safe spot enemies couldn't go onto)). It would be good to introduce more power-ups (a green shell that the player throws against enemies for instance) in order to solve this issue (see [this section](https://github.com/sebranly/video-game-tester/blob/master/README.md#evolution)). By making the code open-source, developers could submit a PR introducing such a change (see [this section](https://github.com/sebranly/video-game-tester/blob/master/README.md#open-source)).
- :egg: No real secrets in the game like easter eggs or hidden levels that get unlocked after completion
- :feelsgood: It would be good to have some levels that feel like an adventure in the way that a particular level has a starting point and the player has to reach the ending point by following a specific linear path with some challenges in between.

## Super Pokemon Run

### Description

:runner: Crossover between Super Mario Run and Pokémon as a 2D-game

- 👨‍💻 **Author:** Anthony Khelil ([@anthonykhelil](https://twitter.com/anthonykhelil/status/1076856737641230336))
- :calendar: **Release Date:** December 23, 2018
- :mag: **Dates of the test:** End of December 2018 (version Alpha) on Mac
- :arrow_down: **Download Link:** https://www.anthony-khelil.com/SuperPokemonRun/Download.php

### Disclaimer

I didn't finish the game up to 100%. For instance, I didn't test the online mode, hardly tested the endless solo mode, and although I completed all adventure levels, I didn't try to get all special coins for each of them. If some points below are incorrect please let me know. Keep in mind that this is the version alpha of the game so having bugs is understandable.

**For all pros and cons, don't forget to also check out the [All Games Table](https://github.com/sebranly/video-game-tester/blob/master/README.md#all-games-table)**

### Pros

:white_check_mark: Nice things:

- :1234: There is a high-score panel appearing at the end of the level (I'm not sure if this is hardcoded or the scores are being retrieved online but in both cases it's a nice addition)
- :turtle: Speed is being adapted when the player is underwater
- :gemini: Being able to switch characters (Pokemon) to reach points is an interesting part of the gameplay

### Cons

:x: Things that could be improved:

- :abc: Some French mistakes: it should be `Choisissez` and `Labyrinthes mortels`
- :video_game: Controls are frustrating for the attack move and bouncing on walls to switch direction. It should be two handled with two different keys on the keyboard rather than trying to combine everything under one key.
- :snail: Having to wait for a whole "new loop" when we miss a jump is frustrating. In Super Mario Run this is nicely handled by making Mario run a bit on the left before switching back to running towards the right. This wouldn't fit Super Pokemon Run but something similar needs to be implemented. Additionally, the game speed is pretty slow.
- :question: The special coin in level 4 cannot be completed because once falling back in the pool the musical note trampoline doesn't enable the player to jump back on the platform on the left
- :boom: In the adventure mode, after every game over the application crashes (this is not happening for the endless mode)
- :thinking: Some collisions are badly handled: enemies can walk far too much beyond the extremities of platforms, and when the player goes onto an enemy it doesn't kill it like in Mario ; instead the player would float above the enemy, which doesn't feel natural at all. Similarly, exploding a brick with an enemy on top doesn't kill the enemy.
- :rewind: There is no button to retry a level immediately
- :fire: Fire-type Pokemon can go into water but the reverse is not true (inconsistency). Similarly, it feels weird being killed when falling into the void as a fire-type Pokemon because the void is filled with lava.
- :negative_squared_cross_mark: Getting a high-score is too easy because there is no time restraint so the player just has to loop back into the level to get the missing coins. In Super Mario Run this is not possible.
- :eyes: Some visual bugs/improvements (minor bugs):
  - Toad is still unhappy even when we saved him
  - the design of the cage for Toad could be improved
  - water and lava sprites should be animated
  - on the high-score panel, my name appeared on the 3rd slot and all other slots were empty
- :bug: Some major bugs:
  - in the endless modes, Medium and Hard difficulty cannot be played but are still available as an option. When launching them, the player dies instantly after spawning into a level full of a new type of Pokemon. It looks like it won't bug in the final version but for now, these options should be locked in the alpha version.
- :arrow_forward: When keeping moving after being paused by a pausing block, hitting the `Space` key makes the player jump although in Super Mario Run it doesn't
- :mushroom: When a life is lost, it is not reflected on the player like it does in Mario (by changing his size from Tall Mario to Small Smario). It would be a nice addition because it adds a new dimension to the gameplay.
- :first_quarter_moon: Special Coins always appear in the same order on the board when obtained. It would be better to make them appear depending on their position in the level. For instance if there are 3 special coins in the level and the player only got the last one, it would be better to display it as `_ _ *` instead of `* _ _` so that the player has a clue suggesting the other special coins were earlier in the level (it's something I wish I had in "Under the sea" level for instance)