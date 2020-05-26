# DKC1-Entrance-Randomizer

*****************************************************************************
* _____ _      _____  ____  ____  _      ____  _____                        *
*/  __// \  /|/__ __\/  __\/  _ \/ \  /|/   _\/  __/                        *
*|  \  | |\ ||  / \  |  \/|| / \|| |\ |||  /  |  \                          *
*|  /_ | | \||  | |  |    /| |-||| | \|||  \_ |  /_                         *
*\____\\_/  \|  \_/  \_/\_\\_/ \|\_/  \|\____/\____\                        *
*                                                                           *
* ____  ____  _      ____  ____  _      _  ____  _____ ____                 *
*/  __\/  _ \/ \  /|/  _ \/  _ \/ \__/|/ \/_   \/  __//  __\                *
*|  \/|| / \|| |\ ||| | \|| / \|| |\/||| | /   /|  \  |  \/|                *
*|    /| |-||| | \||| |_/|| \_/|| |  ||| |/   /_|  /_ |    /                * 
*\_/\_\\_/ \|\_/  \|\____/\____/\_/  \|\_/\____/\____\\_/\_\                *
*****************************************************************************

  ______  _                                                    ___ 
 / _____)| |                                                  / __)
| /  ___ | |  ___    ___   ___   ____   ____  _   _     ___  | |__ 
| | (___)| | / _ \  /___) /___) / _  | / ___)| | | |   / _ \ |  __)
| \____/|| || |_| ||___ ||___ |( ( | || |    | |_| |  | |_| || |   
 \_____/ |_| \___/ (___/ (___/  \_||_||_|     \__  |   \___/ |_|   
                                             (____/                
 _______                                                           
(_______)                                                          
 _         ____   ____  ____    ___                                
| |       / _  ) / ___)|    \  /___)                               
| |_____ ( (/ / | |    | | | ||___ |                               
 \______) \____)|_|    |_|_|_|(___/                                
                                                                   
	- ROM: Read Only Memory (the format all games are in)
	- Seed: A randomizer term. Basically, if two ROMs have the exact same seeds, they are identical. A technical definition is "A random seed (or seed state, or just seed) is a number used to initialize a pseudorandom number generator."
	- Logic: Another randomizer term. Logic ensures the seed is completable.
	- Exit: A way to exit the current stage you are in. NOTE: This is not an exit randomizer! Exit examples: 1-1 exit, 1-1 bonu 1, 1-1 bonus 2
	- Entrance: Any entrance to a stage. A bonus exit leads to a stage entrance. Entrance examples: 1-1 star, 1-1 from bonus 1, 1-1 from bonus 2
	
This is an entrance randomizer. What this means, is the entrances from each exit are randomized. There are a few types of exit. Bonus tokens, bonus rooms, warps, and level exits. This game ends up being a puzzle, now. As is mentioned laterm the goal is to beat 4 bosses and K Rool.

	
This program takes a DKC ROM, randomizes it, and creates a new ROM for you. This program accepts only a U 1.0 version of this game. An error will be thrown if you provide anything else. Also important, is the extention of your ROM. You could have either an sfc or smc. sfc is the standard/official (Super FamiCom) ROM, and shouldn't have a 512-byte header at the beginning of the file. smc is an unofficial but popular extension (Super MagiCom, a copier), and will probably have a 512-byte header at the beginning of the file. In this case, this program accepts both sfc and smc. 


 _     _        _                  _______  _      _       
| |   | |      (_)                (_______)| |    (_)      
| |   | |  ___  _  ____    ____    _       | | _   _   ___ 
| |   | | /___)| ||  _ \  / _  |  | |      | || \ | | /___)
| |___| ||___ || || | | |( ( | |  | |_____ | | | || ||___ |
 \______|(___/ |_||_| |_| \_|| |   \______)|_| |_||_|(___/ 
                         (_____|                           
BEFORE USE
It is best to organize your folder like in the picture (https://imgur.com/a/zjeYb2L). Have a DKC ROM by itself somewhere. This is important as this program will generate a bunch of files for you. 

Now, open the program. On launch, a blank box appears except for a 'file' menu. The menu has 3 options: Load, About, and Exit. Click load. A pop-up will spring up prompting you for a ROM. Navigate to the folder you just set up and select the ROM. On file load, a bunch of options appear (see the included image https://imgur.com/a/9vmxJda).
From left-to-right, we start with the logic. Logic (as explained above) ensures that a ROM's seed is completable. 'No Logic' just means this check is never made and may not be completable. It is highly recommended that you run on logic (for race settings at least).
Next, is seed input. Don't worry about filling this out at first. This is optional. This will be explained after.
Continuing, we have a variety of checkboxes. This is the main area you are interested in. Here, you can select options of how you want your gameplay experience altered. Options include:
	- Low gravity: not truly low gravity. Just higher jumps, essentially.
	- Music: Randomizes which tracks play on which stages.
	- God Awful Music: Plays tracks using the wrong instruments.
	- Bosses: Randomizes what occurs in each boss.
	- Enemies: Randomizes most enemies.
	- Animal buddies: Randomizes each animal crate to be one of the 5 buddies (Yes. Squawks too).
Finally, we come to a color drop-down. Here, you can select a color scheme to use.
	- Red: Gives the monkeys red (original) clothing
	- Teal: Gives the monkeys teal clothing
	- Purple: Gives the monkeys purple clothing
	- Green: Gives the monkeys green clothing
	- White: Gives the monkeys white clothing
	- Yellow: Gives the monkeys yellow clothing
	- Orange: Gives the monkeys orange clothing
	- Albino: Gives the monkeys a red aura along with red eyes
	- Ghost: Turn the monkeys all white
	- Random: Selects one of the above at random
In the lower left-hand corner, there is a checkbox entitled 'Randomize ROM.' This is primarily useful to race organizers. This lets you generate all the files listed below, except for a ROM. This should be left checked 99.99% of the time. 
After you complete these areas, click the 'Randomize' button. Your folder you set up before will now look like this (https://imgur.com/a/SLc97n0)

Make sure you click the Candy picture!

Now, at the end of your ROM files is the seed number (See image https://imgur.com/a/LIUlSMg). If you have a particularly fun run and want to share with your friends, you can give them just the seed number. They can input this in the designated spot, and as long as logic matches, they can get the same experience as you with differnt settings! This is good for races, where you can have different racers choose different colors but have the same seed! Also, the 'God Awful Music' option applies to this. Really any option. So, for those who are a little hesitant, you can choose no 'God Awful Music' but you friend can.


 _______  _  _                                                         
(_______)(_)| |                                                        
 _____    _ | |  ____                                                  
|  ___)  | || | / _  )                                                 
| |      | || |( (/ /                                                  
|_|      |_||_| \____)                                                 
                                                                       
 ______                                                                
|  ___ \                                                          _    
| | _ | |  ____  ____    ____   ____   ____  ____    ____  ____  | |_  
| || || | / _  ||  _ \  / _  | / _  | / _  )|    \  / _  )|  _ \ |  _) 
| || || |( ( | || | | |( ( | |( ( | |( (/ / | | | |( (/ / | | | || |__ 
|_||_||_| \_||_||_| |_| \_||_| \_|| | \____)|_|_|_| \____)|_| |_| \___)
                              (_____|                                  
Starting from the top, we have a new folder called 'ROMs'. This is important. This is where the new randomized files go. Each file is titled with the version, date, and seed number. This is so multiple seeds can be generated at the same time.
Next we have a folder titled 'Spoiler Logs'. This folder is organized by seed. Each spoiler log tells you how to get to a variety of locations. Those locations are:
	Candy
		-Candy W1
		-Candy W2
		-Candy W3
		-Candy W4
		-Candy W5
		-Candy W6
	Cranky
		-Cranky W1
		-Cranky W2
		-Cranky W3
		-Cranky W4
		-Cranky W5
		-Cranky W6
	Funky
		-Funky W1
		-Funky W2
		-Funky W3
		-Funky W4
		-Funky W5
		-Funky W6
	Common hubs
		-Manic Mincers
		-Orang-utan Gang
		-Animal Token Room
	Bosses
		-King K Rool
		-Gnawty
		-Necky
		-Bumble B Rumble
		-Boss Dumb Drum
This way, you can elect not to spoil yourselves completely and just look up the way to Cranky for a hint, the way to Candy for a quick spin in her save barrel, or the way to Funky/some big hubs for more areas to try. Or you can completely give up and look up bosses. All of these routes are unique save for Mincers and Ogang. Those two are not unique because there are multiple entrances to each. Each of the two exits to Funky are unique.
Next, we have 'DKC cheat sheet (token areas).txt'. This file is simple. This is organized by animal token and tells you from which entrances these are obtainable.
Finally, we come to 'DKC note aid.txt'. This file just lists every available entrance.


  ______                              _               
 / _____)                            | |              
| /  ___   ____  ____    ____  ____  | |  ____  _   _ 
| | (___) / _  ||    \  / _  )|  _ \ | | / _  || | | |
| \____/|( ( | || | | |( (/ / | | | || |( ( | || |_| |
 \_____/  \_||_||_|_|_| \____)| ||_/ |_| \_||_| \__  |
                              |_|              (____/ 
It's time to run this! Open up this ROM in the platform of your choice and start the game. You will immediately notice something odd after you select one player (NOTE: This will break on 2-player contest). There is no Donkey Kong sprite on the world map! Also, there is an odd-looking seed number. This just says what flags are set up for this run. You never have to worry about any of the text from the first dash onwards. World map has effectively been removed from this. You start in Jungle Hijinx. The treehouse and Banana Hoard are the same. This is intentional. Everything revolves around 1-1.
Bonuses are removed, but not the bonus wall or cannon! You just won't have to go to bonuses. In an unrandomized setting, 1-1 bonus 1 exit will spit you out at 1-1 bonus 1 entrance.
Start select, while normally takes you back to the world map, here just brings you to your last checkpoint. If no checkpoint is set, this takes you back to the start of 1-1.
In your travels, you might encounter Cranky, Candy, or Funky (aka your Kong family). There are 6 varieties of each one, based on the fact that there are 6 in the original. Saving your game at a Candy is useful. Saving will automatically start you at the next entrance on reset. Also, loading from a save clears your checkpoint. Additionally, Candy saves your bosses cleared, so you never have to worry about resetting after saving. Cranky offers you hints. Be careful to read carefully! These hints are not always how they seem! Each Funky offers two distinct exits. You can take a ride in his bodacious barrel, or just walk away.
All exits are unique, but not every entrance is! For example, think of 1-1. Bonus 1 could take you to Elevator Antics (Antics). 1-1's Bonus 1 will always take you to Antics, no matter how you get to 1-1. Now, 1-1's exit can also lead to Antics. In each case, you are going to the exact same version of Antics.

***WARNING***
Do not touch swap on entering. Rare, but you could hardlock the game!


 ______                                  
(____  \                                 
 ____)  )  ___    ___   ___   ____   ___ 
|  __  (  / _ \  /___) /___) / _  ) /___)
| |__)  )| |_| ||___ ||___ |( (/ / |___ |
|______/  \___/ (___/ (___/  \____)(___/ 
                                         
There are 4 'world' bosses and 1 King K Rool. You must defeat all of the 4 bosses for King K Rool to appear. But worry not! All bosses are replaced by a barrel once you defeat them, so no re-fighting bosses. If you find King K Rool early, however, a mincer replaces him to reset you at last checkpoint.
The four bosses are Gnawty, Necky, Bumble B Rumble, and Boss Dumb Drum. There are no repeat bosses like in the original. Only 1 Gnawty and 1 Necky.
Also, once you find a boss, you automatically keep restarting it until you win. Start select still works in bosses, but instead of restarting from the last checkpoint obtained, you are restarted at the boss entrance. But no need to fear! Your checkpoint is still safe and will be put back after you leave the boss room!
Further, please note that every boss, on defeat, warps you back to 1-1. This is intentional, as it makes using the spoiler logs easier. As noted before, though, your checkpoints are still intact!


  ______                _ 
 / _____)              | |
| /  ___   ___    ____ | |
| | (___) / _ \  / _  || |
| \____/|| |_| |( ( | || |
 \_____/  \___/  \_||_||_|
                          
The goal of this is to reach the credits. You do this by defeating King K Rool (which requires you to beat 4 other bosses).


 _     ____  ____  ____  _____  _____ ____ 
/ \ /\/  __\/  _ \/  _ \/__ __\/  __// ___\
| | |||  \/|| | \|| / \|  / \  |  \  |    \
| \_/||  __/| |_/|| |-||  | |  |  /_ \___ |
\____/\_/   \____/\_/ \|  \_/  \____\\____/
                                           
Now in SpoilerLog.txt, you are told where tokens lead you. This is purposely left vague. If you get a particularly hard/annoying seed, you can see if tokens led to bosses.
Also, now a number is always shown at the top of the screen. This number tells you what world you are currently in. This is useful for Cranky hints!
Additionally, in the lower-left corner of the screen is a boss tracker. This is blank at first, and as you beat bosses, the world number appears. This way, if you reset, you always know what bosses you still need. This only appears when lives change! 
	For example, if you see '12 5' in the lower left, you know you still need Queen Bee.
Bosses by world:
1 - Gnawty
2 - Necky
3 - Bee
5 - Drum

Quick deaths are now a thing! And now you have truly infinite lives.
