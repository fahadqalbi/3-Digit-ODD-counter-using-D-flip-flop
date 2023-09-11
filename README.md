# 3-Digit-ODD-counter-using-D-flip-flop
In this digital logic design project, I have made a 3-digit odd counter using D-Flip Flops to make the counter. This counter has features like:  User desired input, Pause option, Reset option

Warning/Note


Note: always use resistors to apply active ground at pins of the ICs which require active low logic or at all the inputs to provide zero. otherwise IC will put out garbage values.

Note: please use a proper 5V power supply that has plenty of juice in it so that all the logic ICs perform as intended. I use an arduino to provide power.

Things required for this projects are:

D-Flip Flop ICs
AND Gate ICs
OR Gate ICs
NOT Gate ICs
555 timer IC
Resistors for generating Clock and for providing active ground
Capacitors for generating Clock
4-bit Bit Switches
7-Segment Displays
Binary to Seven Segment Decoder ICs
BCD Counter ICs
Push Button (toggle)
ON/OFF slide Button
Jumper Wires
Bread Board
Note: You can use 3-way AND & OR gates, they weren't available to me so i use the 2-input ones.

First of all we will write down all the states for our counter. 
That is how our odd counter using D-Flip Flops will initiate and continue. 
To make a 3-digit odd counter we only need the to change the 1st digit on ones decimal place to odd number. 
That will be the counter starts from 0 and then goes to 1,3,5,7,9 and then again at 1 not zero i.e. because its an odd counter.
Now for the tens and hundreds decimal place we will use simple BCD counter IC to count from 0 to 9, the clock for this IC will come from the odd counter, basically we will cascade 2 BCD counters with the ODD counter.
