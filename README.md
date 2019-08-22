Yu-DeSSE - Yuvi Demon's Souls Server Emulator Fork

New updated Demon's Souls Server Emulator that is being used on https://TheArchstones.com (currently the most popular DeS Server)

This includes a wealth of upgrades,
1) User Selectable World Tendency, 
	Uses the sqllite DB for tracking this, Along side this is a Server management tool I developed to easily modify the sql table for anyone. But of course in game users can lay down certain messages to change there own world tendency
2) Northen Limits the unrealeased area is now playable via multiplayer to those with Debug units. (https://www.youtube.com/watch?v=rEdtoI3mzWg -  a player made a stream about this.)
3) Longer list of Player location presented to users.
4) Status is printed to a html page so users can view live stats online.
5) Some misc. code improvements that i can remember, This was developed over another year. 

This code has been operating stable for over a year now. More improvements to come with additonal features to be added.
Some prelim work is done for this. 


Requirements are the following
1) Dns proxy configured, You can use python DNS Proxy or Windows DNS Server which I ran for awhile.
2) python 2.6/2.7
3) pycrypto 

Setup:
After you have DNS Server running, Configure you Info.ss to your external IP.
Then run the emulator.py


Oringinal Info:
This is a very quick and dirty server emulator that supports the most basic features.
Working at the moment:

 - matchmaking (only internally in each region, EU/US/JP people won't see each other's summon signs for example)
 - messages, pre-seeded with some old EU messages, but new messages have priority
 - ghosts
 - bloodstains, pre-seeded with some old EU stains, new stains have priority
 
The matchmaking only works by virtue of Sony's matchmaking servers being online. I don't know
if these servers are generic and will continue working in the future or if they might
be turned off at some point. It works right now, at least.
