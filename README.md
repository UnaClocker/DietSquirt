# DietSquirt
Low cost DIY open source MegaSquirt derivative.

Welcome to my incomplete project. This was meant to be a much cheaper 
alternative to MegaSquirt. It uses the same processor as the MegaSquirt,
which is wired the same way as you might wire it for MegaSquirt-Extra 
firmware. Now being that this is not a licensed board, you shouldn’t run 
their firmware on it. But if you do, who am I to stop you. ;) You’re not 
supposed to run MegaSquirt on street cars either, but most MegaSquirt users 
do.

Please watch the video about this: https://www.youtube.com/watch?v=LJTZ3sH1d-M

This project is licensed under the BSD License. Take it and do anything with
it. If you mass produce and sell it, I hope you’re not using the MegaSquirt 
firmware, their lawyers will bury you. Your own personal use, totally another 
matter, not worth coming after Joe Blow who’s running it in their own car. 
Ideally, the MegaSquirt firmware can prove the board, then we can switch to 
a far better processor and far more open firmware like the STM32F4 with 
RusEFI firmware. I signed the board “Anonymous” because of the risk of 
B&G’s lawyers. 

As stated, this board is a work in progress. I’d like to say I can come 
back and finish it, but I designed it two years ago, maybe 2 1/2 years at 
this point. Right after that I discovered my wife was having an affair 
(TMI…), and entered a long drawn out divorce. Now I’m a single father of 
two kids so I don’t have much time to devote to these projects anymore. 
I’m placing the files on Github, we can work together to update and fix 
the board as testing progresses.
Current known issues: 
	The components for the voltage regulator circuit are too big and 
don’t fit. Namely the capacitors. 
	It needs the LC filter added between the output of the VR and the 
rest of the board to clean up the noise from the switch mode power supply. 
See the data sheet to the 34063 voltage regulator for that circuit.
	The DB15 and DB25 connectors are too far inboard, they need to be 
shifted out to the next mark on the silkscreen.

Next up, this board does not have onboard injector drivers. I had intended 
it to use the JBPerf P&H board. He seems to have stopped selling it since 
then, so I, or someone else may need to create a clone of his old board. 
It’s a very very simple circuit board to make. The chips are still available.

You can submit the .brd files to OSHPark.com to have 3 copies of the board 
made. It’s VERY expensive there. but if you’re in the US, they’re very fast. 
You can get 10 boards made at www.elecrow.com, under their 5cmx10cm pricing, 
I believe it’s $20 for 10 boards. Give the spare boards to friends, or save 
them as spares. Don’t sell them, you’ll risk the wrath of the B&G lawyers.

See the attached BOM for the list of parts you’ll want to order from Digikey 
for this board.

The files are for Eagle. Place the .brd and .sch files in a DietSquirt folder
under your main eagle projects, then load the .sch schematic file and .brd board 
layout file. The gerbers are included, but since the board needs work still, 
I wouldn't suggest building having it produced. At the very least, you'd have 
to run an external 5v voltage regulator. I'd have prefered to have done the 
board in KiCad, but I knew Eagle better at the time. You can get a free version 
of Eagle, google it, download it. Works in all 3 major OS's.

I’m probably forgetting a lot. I’ll document more as time allows. 
Questions? unaclocker@gmail.com
