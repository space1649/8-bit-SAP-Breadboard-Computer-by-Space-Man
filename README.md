# 8-bit-SAP-Breadboard-Computer-by-Space-Man
This is my build of Ben Eater's 8-bit breadboard computer

Ben Eater SAP 8-bit computer diagram 4-9-2017.vsd  This is a MS Office Visio file  (.vsd). You can get a Visio viewer if you don't have Visio. 
I included an XPS file format as well. Using the visio file you will find it helpful when building it as you can highlight a connection line and it will show you the two connection points.

List of Issues encounter building the computer


Adder Circuit 3-10-2017 ( Reversed Data Lines )
Clock Crcuit 3-13-2017 (1 MEG Resistor connected to 5v not Ground)
Clock Circuit – Debounce adjustment  need .5 decond delay ( 1uf x 470K = 470ms)
MAR MI   Address Lines reversed
PC – Added Clear Signal
OP Code – Reset was tide to HIGH Causing count to 7 not 5
Added Reset Buttons
RI needs to be High to Write to RAM, Since a NAND gate inverts the signal w/Clock
Corrected Jump Circuit Only One Nand gate IC ( 4 Nand Gates Used)
Fixed RAM Write issue - Needed to isolate the clock from the RC circuit. Fixed feedback noise
Added 10K Resistor to Write button in Program Mode (Pullup to 5 v instead of Floating)

Added RC Circuit to absorb spikes during switching between Run and Program mode. (Noy in Picture but in Diagram)
This Fixed issue where switching between Run and Program mode caused Memory Write signal to go low clearing RAM contents.
