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

An important characteristic of op amps is that they are direct-coupled or dc amplifiers, where dc stands for direct-coupled (it could equally well stand for direct current, since a direct-coupled amplifier is one that amplifies signals whose frequency is as low as zero). Ideal op amps will amplify signals of any
frequency with equal gain, and are thus said to have infinite bandwidth.

<img src = "https://user-images.githubusercontent.com/91787553/227756072-67d4b261-ea5b-4df5-9ba7-271759475884.png" width = 400>

where,
vIcm = 1/2 (v1 +v2) and vIcm is the common mode input signal
vId = v2 −v1 and vId is the differential input signal

<h3>Inverting Configuration</h3>
In an inverting configuration, the input signal is connected to the inverting input terminal (-) of the op amp, and a feedback resistor is connected between the output and the inverting input terminal. The non-inverting input terminal (+) is connected to ground.

The input signal is amplified and inverted at the output, meaning that the output signal is equal in magnitude to the input signal, but with the opposite polarity. The gain of the amplifier is determined by the ratio of the feedback resistor to the input resistor.

The inverting configuration is often used in applications where a negative voltage gain is required, such as in audio amplifiers or filters. It can also be used as an inverting buffer, which is a circuit that produces an output signal that is a replica of the input signal, but with a different impedance or current capability.

Overall, the inverting configuration is a versatile and useful circuit configuration that allows for a wide range of applications with op amps.

<img src = "https://user-images.githubusercontent.com/91787553/227757227-bc585220-b6c5-4efc-9d0b-157e16921d88.png" width = 400>

<h3>The Closed Loop</h3>
Due to the high gain of the op-amp, the voltage at the inverting input terminal (v1) is effectively forced to match the voltage at the non-inverting input terminal (v2). This is known as virtual short circuit because it appears as though the two input terminals are shorted together, even though they are not physically connected.

In the case where v2 is grounded (i.e., v2=0), the op-amp output will be negative and v1 will also be forced to zero. Therefore, we refer to the inverting input terminal as a virtual ground, as it appears to be at zero potential even though it is not physically connected to ground.

It is important to note that while the concept of virtual short circuit and virtual ground can be useful in analyzing op-amp circuits, it is not appropriate to physically short circuit any circuit components. Doing so can result in damage to the circuit and potentially cause harm to the person conducting the experiment.

<img src = "https://user-images.githubusercontent.com/91787553/227757620-8eb375c0-6f40-4762-ac29-47417165cb1b.png" width = 400>

<h3>Effect of Finite Open-Loop Gain</h3>

The output voltage vO, then the voltage between the two input terminals of the op amp will be vO/A. Since the positive input terminal is grounded, the voltage at the
negative input terminal must be −vO/A. 
i1 = vI −(−vO/A)/R1 = (vI +vO/A)/R1
G ≡ vO/vI = (−R2/R1) / 1+(1+R2/R1)/A

<img src = "https://user-images.githubusercontent.com/91787553/227759153-4204a1e8-77df-47b7-8913-efed64fe2729.png" width = 400>

<h3> Weighted Summer </h3>
The resistance Rf in the negative-feedback path (as before), but we have a number of input signals v1,v2,...,vn each applied to a corresponding resistor R1,R2,...,Rn, which are connected to the inverting terminal of the op amp. 

<img src = "https://user-images.githubusercontent.com/91787553/227816861-fd29985a-ee2f-4a2e-8048-0d9fbf1ceaec.png" width = 400>

The output voltage is a weighted sum of the input signals v1,v2,...,vn. This circuit is therefore called a weighted summer. Note that each summing coefficient may
be independently adjusted by adjusting the corresponding “feed-in” resistor (R1 to Rn). This nice property, which greatly simplifies circuit adjustment, is a direct consequence of the virtual ground that exists at the inverting op-amp terminal. 

<img src = "https://user-images.githubusercontent.com/91787553/227817033-9429e2b5-8e08-465d-97ec-4d46dae17a10.png" width = 400>

Hence the weighted summer is capable of implementing the summing coefficients of both the signs

<h3> Differential Amplifier </h3>

The differential amplifier is a voltage subtractor circuit which produces an output voltage proportional to the voltage difference of two input signals applied to the inputs of the inverting and non-inverting terminals of an operational amplifier.

Thus far we have used only one of the operational amplifiers inputs to connect to the amplifier, using either the “inverting” or the “non-inverting” input terminal to amplify a single input signal with the other input being connected to ground.

But as a standard operational amplifier has two inputs, inverting and no-inverting, we can also connect signals to both of these inputs at the same time producing another common type of operational amplifier circuit called a Differential Amplifier.
Then differential amplifiers amplify the difference between two voltages making this type of operational amplifier circuit a Subtractor unlike a summing amplifier which adds or sums together the input voltages. 

<img src = "https://github.com/Suraksha-Rajagopalan/Op-Amp/assets/91787553/aead1ba2-8fe0-477b-876b-75407e887752" width = 400>

<h3> Instrumentational Amplifier </h3>

<img src = "https://github.com/Suraksha-Rajagopalan/Op-Amp/assets/91787553/8105492b-8769-46fa-99ae-b70c8ef0d4fe" width = 500>

In-amp just provides the difference between two voltage sources with a gain that can be set by an external resistor.

<h3> Integrator Circuit</h3>
An integrator circuit is a type of inverting amplifier where the feedback resistor is replaced with a capacitor of suitable value. It is designed to produce a triangular wave output from a square wave input. Integrator circuits can be configured to perform calculus operations such as differentiation and integration. A passive integrator does not use any active devices like op-amps or transistors but only passives like resistors and capacitors. An active integrator provides a much lower output resistance and higher output voltage than it is possible with a simple RC circuit. The construction of a simple integrator circuit using op-amp requires two passive components, a resistor and a capacitor, which form a first-order low pass filter across the active component Op-Amp.

<img src = "https://github.com/Suraksha-Rajagopalan/Op-Amp/assets/91787553/8105492b-8769-46fa-99ae-b70c8ef0d4fe" width = 500>
