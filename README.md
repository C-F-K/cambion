# cambion

## because why settle for games that kind of do what you really want but piecemeal and incompletely

### concept

you're a changeling (the d&amp;d kind, latter-day offspring of humans and doppelgangers, with some homebrew headcanon of being somewhat intrinsically aberrant); you find yourself in a strange city and you get to decide what you do with yourself. you do have to eat, drink and sleep though (tbh why wouldn't i add potty breaks as well, like in The Ship). also if you move out of your starting digs you'll need to either own the place or pay rent. there are only so many hours in a day and things will progress (or go on as usual) without your input. there are some other changelings in town, known only to each other, who have a small amount of narrative drama going on between them which you're entirely free to ignore. the other changelings will teach you their skills, though.

#### why a minecraft mod?

so i can bake my apple pie from scratch without having to invent the universe. sorry prof sagan. (also i code java for a living.) it's probably going to be more of a total conversion eventually, though.

#### isn't this just kind of a capitalism simulator? do jobs, pay rent, eat and sleep, bla bla bla

yeah i guess you can look at it that way. idk how else you want to implement an immersive sim/survival game in an urban environment, though. a survival game that takes place under socialism/communism would take the challenge out of the survival aspect.

### aspects and related todos

the central fun generator is what i'm pretty sure is baked into every game on some level but which i'm here making explicit: figuring out how stuff works. random generation ensures that for every world you generate, stuff will work differently, but you'll be able to essentially apply the scientific method to figure it out.

#### roguelike

	* survival mechanics (hunger, thirst, fatigue, bathroom)
	* permadeath
	* day/night cycle
	* The Six Stats, which may influence *some* things randomly but, like, it shouldn't be possible to have good Str but roll a nat 1 while climbing and fall
	* probably adapt the body slot system from Space Station 13
	
#### changeling 

	* shapechanging, of course
	* take ~6 seconds to change physical appearance + gender pronouns + voice
	* keep a short "favorites" list of, say, 5 or so frequently-used appearances; also always re-select the 5 or so most recent appearances used
	* build on the body slot system so that you can steal people's mundane clothes, armor, or both
	* you have to listen to someone speak for a while to be able to mimic their voice, otherwise you have a chance to arouse suspicion
	* similarly, you have to have some privacy and quiet to study someone's body in order to mimic their appearance perfectly
	* Lovecraftian Hidden Fun Stuff woOooOoOoOo~ 

#### assassin

think Dishonored, but randomly generated. how do you get from A to B, deal with the target (which might be an assassination but also theft, kidnapping, leaving a message, other kinds of shady business), and get back without being noticed? this will require:
	* a more involved stealth system (light level already exists in vanilla minecraft, as does line-of-sight i think; will also need noise level and NPC reactions based on where you are and what you're doing) 
	* various move modes (crouch, walk, run, sprint)
	* something very much like parkour (climbing, mitigating fall damage, "flow" like Mirror's Edge)
	* missions/jobs
	* the city (see below)

#### alchemist

think The Witcher, but deeper. what substances have what properties and what processes have what effect on them?
	* animal/vegetable/mineral (hunt animals, gather/cultivate plants, prospect for minerals)
	* classical western alchemical bases/reagents etc 
	* also classical alchemical processes (wikipedia outline of alchemy has a good list)
	* plenty of d&amp;d source material to implement here too

#### mage

think d&amp;d, but instead of just getting spells for free as you level up, you actually research them.
	* material/verbal/somatic/focus components
	* materials as described under alchemy
	* verbal components: syllabary?
	* somatic components: gestures, possibly derived from ASL?
	* focus components: rare items, but maybe also geometric diagrams a la fullmetal alchemist tbh (makes more sense as explicit magic than as "alchemy")
	* basically have it operate like alchemy tbh; components have properties, combine them like legos, note down the results, rinse and repeat
	* plenty of d&amp;d sourcebooks have expanded on how exactly players can invent new spells, including a sort of morphology of spell mechanics

#### tinker

basically doing Piero's job in addition to Corvo's tbh
	* mechanical (gears, springs, some analytical engine type shit)
	* electric? very very basic if so
	* steam, for larger constructions (this is probably strictly optional to even add to the game) 
	* as above (with magic and alchemy), except you disassemble devices to find out how to make similar things? idk this honestly seems like the hardest part to code
	* the main thing i'm thinking of is disassembling, like, a regular crossbow and some other devices to discover how to make + improve a hand crossbow, but obvs you should actually be able to invent other things too

#### the city

the environment is really a very large NPC that should have a life of its own and react to your action or inaction. will need:
	* npc scheduling
	* some kind of NPC simulation that isn't quite as involved as stabbing individual organs in Dwarf Fortress but allows more nuanced interaction than point-click-blarg-ded
	* a whole entire utility for actually generating a city layout, districts, individual buildings, rooms in buildings, et cetera ad infinitum...
	* a political economy, including industries and related npc jobs (most of which you can probably do yourself too, for safe mundane income)
	* npc agendas (stuff that motivates people outside of immediate survival, influencing their daily routines) 
	* npc quirks (exploitable for assassin purposes; steal a guy's tobacco to make him smoke your poisoned cigar idk)
	
### disclaimer

you are not guaranteed to have fun playing this because i am a nerd with very particular tastes; statistically though there have to be a few people enough like me that they'll also enjoy it.

### disclaimer the second

i am not tarn adams, the brilliant mathematician; i have a day job and i am not committing to a 20-year roadmap because i want to *play* this game ASAP. as such i'm going to be cribbing *shamelessly* when and wherever i can. the cool thing about copy-pasting other people's code is that you still have to understand how it works or it won't. if i crib from you and forget to credit you in the comments, drop me a line.