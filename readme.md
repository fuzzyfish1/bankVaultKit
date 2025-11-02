TODO:
	ADD license

proposed Structure:
	.gitignore
	License
	Kit1
		//Hardware to buy somn.md
		//Manufacturables
		//lesson plan
	Kit2 : etc.
	src/


# BANK VAULT PROPOSAL
Inspired to make this kit as Andy told me he wanted to do a bank vault project with a password. I wanted to make the lesson plan have a concept as a preface to something kids do with their hands focusing on teaching to think like engineers, then practicing doing that engineering and using that hands on work to help them catch up to some more grand concept. I think this approach is a great way to perhaps bridge younger kids to more difficult/time consuming projects shows very well how to break down a project into smaller ones. Made this doc especially because of the confusion/lack not a great teaching plan with the catapult project. 

##Kits features 
I want to make this kit modular and fit with other kits.

- TOP is a coin sorter (DESIGNED), you can slide a coin in it drops into one spot for each coin

- Body/Frame (DESIGNING) (friction fit to the top) is the second part, holds the security system for the coins

- Coin Trays (slide in), uses load cells to measure num Coins as they drop in directly from the coin sorter
## Teaching Timeline
1. Day 1: CAD + manufacturing + money
	* Present them with top half of kit which is the coin sorter
	* Teach them budgeting/saving (prolly one or 2 slides at most)
	* Engineering principles		
		- Tolerance
		- Clearance
		- Types of fits
			- Interference
			- Friction
			- Etc.
	* Manufacturing at scale using these tolerance/clearances
	* Bring https://www.printables.com/model/116911-clearance-tolerance-test 
	* Engineering practice
		- CAD a real coin with calipers or somn
		- Design their own 3d printable coin
		- Design the slide in plate mechanism with custom lettering/design in tinkerCAD
		- Needs to understand the kind of fit they are making, we give them what our tolerances are for laser/print and the rest is easy
	* Play with the coin sorter
2. Day 2: Systems + personal Security
	* Present them with the second half of the kit, the Security/Vault Assembly
	* Teach them abt systems Engineering design principles
		- Introduce Systems engineering
		- Nothing operates as a standalone electrical/CS/mechanical engineering thing but rather a group of systems working together
			- Use our kit as an example, mechanical sorter, CS password ting, electronics for locks, even those are different systems
			- Its turtles all the way down meme but its systems instead lol
		- Designing for a lifecycle
			- What happens when you forget your password?
		- Modular and interchangeable components
			- Easy bc our kit is modular
			- How this affects lifecycle/maintenance etc.
	* Teach them who to give/not to give their passwords to and how secure different things are
		- Don't click on shady links
		- How to convince someone to give you their password
	* Engineering practice
		- CAD something to hold the coins inside the vault that catches the coins, has to fit within our vault and have mounting point for our load cells
		- Build Vault Password security system
		- Display if it works/they can enter using a OLED display or somn (if they have time)
		- Enter a password using buttons or biometric or maybe an NFC password key would be cool etc.
		- Use micro servo locks
		- Their own failsafe in case they can’t access, let them design the algorithm and you help them with implementation
3. Day 3: Software principles, Metrology
	* Engineering principles
		- Datastructures: Arrays OR linear equations (y=mx+b)
			- M ex: weight of coin
			- X ex: num coins
			- B ex: weight of box/initial displacement
			- You could do this instead with an array filled with num coins/bands, useful if sensor is not linear bc then kids can calibrate this by dropping in coins and reading out measurement
		- Tolerances/ranges in measurements
			- Mathematical background in the Central Limit Theorem
				- CLT experiment online
			- Used in constructing confidence intervals
			- You can show that it is statistically likely to be just fine even though potential error/confidence interval increases with numCoins
			- That is why we need a Measurement band (tying the concept to the engineering alg we develop)
		- You could also teach absolute/relative measurements
			- Something cool would be you could show them a space time diagram (without math) to explain “time travel” relative to other frames of reference in time and space (they would understand if you don’t show math and they will think its cool)
			- Absolute including weight of box
			- Relative ex: having to zero our scale + the relative nature of this
		- Error handling/branches/edge cases
			- Every branch needs to be handled for safe code ex: detect if the coin went in the wrong hole
			- Does not need to be a try catch, its probably one extra if statement in our own code, but it teaches programming defensively
	* Engineering practice
		- Using load cells to figure out how many coins there are
		- Finishing what we started last time
		- Mathematics in Code
4. Day 4: summary, finishing things
	* Summarize engineering concepts (one slide each)
		- Metrology + error (how + why we create band for measured weights -> coins
		- Engineering as a system (kit is split into modular parts)
		- products as a lifecycle (forgetting passwords)
		- Personal Security (don't give password to people, shady links etc.)
	* Teaching how to manage money/save/invest
	* Engineering principles
		- Bottom up engineering/ Top down engineering
		- If you were to make this, would you figure out how to make things and what to make out of it … or figure out what you want to make and then how to make it
		- So they can learn the process to figuring things out themselves, how to add to this if they wanted to
		- Anything else needed so they can do it on their own/continue writing software
			- Links to components and what they can do with them they can show their parents (daddy buy me an esp32 so i can attach it to the internet)
	* Demo in front of class
	* Finish everything else
	* Decorate the kits with lego people robbing the vault or somn idk
