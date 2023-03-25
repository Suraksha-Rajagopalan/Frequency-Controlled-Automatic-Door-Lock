<div align=center><h1><strong>Op-Amp</strong></h1></div>

The op amp has three terminals: two input terminals and one output terminal. Terminals 1 and 2 are input terminals, and terminal 3 is the output terminal.
Two terminals, 4 and 5, are brought out of the op-amp package and connected to a positive voltage VCC and a negative voltage −VEE. 
The two dc power supplies as batteries with a common ground. It is interesting to note that the reference grounding point in op-amp circuits is just the common terminal of
the two power supplies; that is, no terminal of the op-amp package is physically connected to ground. 

<div align = center><img src = "https://user-images.githubusercontent.com/91787553/227740132-77dd871c-7de4-4340-a124-ee3734cf8f56.png"></div>

The op amp is designed to sense the difference between the voltage signals applied at its two input terminals (i.e., the quantity v2 − v1), multiply this by a number A, and cause the resulting voltage A(v2 − v1) to appear
at output terminal 3. Thus v3 = A(v2 − v1). 
The ideal op amp is not supposed to draw any input current; that is, the signal current into terminal 1 and the signal current into terminal 2 are both zero. In other words, the input
impedance of an ideal op amp is supposed to be infinite.
The voltage between the ground and the terminal 3 will be same ```Independent of the current``` that may be drawn from terminal 3 (output terminal) into a load impedance. The output impedance of an ideal op amp is supposed
to be zero.
Input terminal 1 is called the inverting input terminal and is distinguished by a “−” sign, while input terminal 2 is called the noninverting
input terminal and is distinguished by a “+” sign.

the op amp responds only to the difference signal v2 −v1 and hence ignores any signal common to both inputs. That is, if v1 = v2 = 1 V, then the output will (ideally) be zero.
This property is called common-mode rejection, and an ideal op amp has zero common-mode gain or, equivalently, infinite common-mode rejection. 

Op amp is a ```differential-input```, ```single-ended-output``` amplifier

<h3> Equivalent Circuit of an Ideal Op Amp</h3>
<div>
<img src = "https://user-images.githubusercontent.com/91787553/227740687-9b517036-ba4b-40d6-93ff-3f721cb44c5c.png" width = 400>
</div>

An important characteristic of op amps is that they are direct-coupled or dc amplifiers, where dc stands for direct-coupled (it could equally well stand for direct current, since a
direct-coupled amplifier is one that amplifies signals whose frequency is as low as zero). 
