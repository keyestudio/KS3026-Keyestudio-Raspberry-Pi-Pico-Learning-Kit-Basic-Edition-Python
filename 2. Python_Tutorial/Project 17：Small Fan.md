# Project 17：Small Fan

1.  **Introduction**

In the hot summer, we need an electric fan to cool us down, so in this
project, we will use the Plus control board to control 130 motor module
and small blade to make a small fan.

2.  **Components Required**

|                                                         |                                      |                        |                         |                         |
| ------------------------------------------------------- | ------------------------------------ | ---------------------- | ----------------------- | ----------------------- |
| ![](/media/bbed91c0b45fcafc7e7163bfeabf68f9.png)      |                        |                         |                         |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 |                        |                         |                         |
| ![](/media/9197d4aff9356c585b7ef68e33a6881d.png)  |                         |
| DC Motor\*1                                             | Breadboard\*1                        | Fan\*1                 | S8050 Triode\*1         |                         |
| ![](/media/7dcbd02995be3c142b2f97df7f7c03ce.png) |
| S8550 Triode\*1                                         | 1KΩ Resistor\*1                      | Jumper Wires           | Diode\*1                | USB Cable\*1            |

3.  **Component Knowledge:**

![](/media/9197d4aff9356c585b7ef68e33a6881d.png)

**Triode：**

It is referred as the semiconductor triode and a bipolar transistor or a
transistor.

The triode is one of the basic semiconductor components as the core of
the electronic circuit., which can amplify current. The triode means
that two PN junctions are made on a semiconductor wafer. The two PN
junctions divide the entire semiconductor into three parts. The middle
part is the base area, and the two sides are the emitter and collector
areas.

As for NPN triode, it is composed of two N type semiconductors and a P
type semiconductor.

The type of transistor which may be used in some applications in place
of the triode tube is the "junction" transistor, which actually has two
junctions. It has an emitter, base, and collector which correspond to
the cathode, grid, and plate, respectively, in the triode tube. Junction
transistors are of two types, the NPN type and the PNP type.

The PN junction between the emitting area and the base area is emitter
junction and the PN junction flanked by the collector area and the base
area is collector junction. And three pins are E（Emitter, B (Base)and C
(Collector).

![](/media/3bace56b6d4c5836d1f334038e88acf1.jpeg)

S8050（NPN triode）

![](/media/3bace56b6d4c5836d1f334038e88acf1.jpeg)

S8550（PNP triode）

The S8050 transistor is a low-power NPN silicon tube and its the maximum
voltage of collector and base can reach 40V and the current of the
collector is (Ic) 0.5A.

The pins of the S8050 transistor should facing down, pin 1 is the
emitter (E pole), pin 2 is the base (B pole), and pin 3 is the collector
(C pole). Similarly, the S8550 transistor is the same.

![](/media/1337a16a23745afe86a78bbc628451f7.png)
![](/media/07ec79528ccc507de5c37057a48595a2.jpeg)

The commonly used triodes are divided into two types: PNP type triode
and NPN type triode. S8550 is the PNP type triode, S8050 is the NPN type
triode, what we provide in this kit are S8050 and S8550.

![](/media/5642275b2be86782bd9563ee840b0d1a.png)

4.  **Connection Diagram 1：**

we apply the S8050(NPN triode) in this experiment to control the motor

![](/media/5db0687f6510b28cf4ccee7aac0d7f93.png)

![](/media/319b4a31b0bc9d65d5f10bfcccf051a1.png)

5.  **Test Code：**

Go to the folder KS3026 Keyestudio Raspberry Pi Pico Learning Kit Basic
Edition\\2. Windows System\\1. Python\_Tutorial\\2. Python
Projects\\Project 17：Small Fan.

You can move the code to anywhere, for example, we can save the code in
the Disk(D), the route is D:\\2. Python Projects.

Open“Thonny”, click“This computer”→“D:”→“2. Python Projects”→““Project
17：Small Fan””. And double left-click the “Project\_17.1\_
Small\_Fan.py”.

![](/media/a5bc848c05c794a4b6b3f91d5310e27d.png)

<table>
<tbody>
<tr class="odd">
<td><p>from machine import Pin</p>
<p>import time</p>
<p>motor = Pin(22, Pin.OUT) # create S8050 object from Pin 22, Set Pin 22 to output</p>
<p>try:</p>
<p>while True:</p>
<p>motor.value(1) # Set motor turn on</p>
<p>time.sleep(4) # Sleep 4s</p>
<p>motor.value(0) # Set motoe turn off</p>
<p>time.sleep(2) # Sleep 2s</p>
<p>except:</p>
<p>pass</p></td>
</tr>
</tbody>
</table>

**6.Test Result 1：**

Ensure that the Raspberry Pi Pico is connected to the
computer，click“![](/media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](/media/5b4104877bd24416f5572a0a161aa6a3.png)

Click“![](/media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts
executing, we will see that The small fan turns for 4 seconds and stops
for 2 seconds. Press“Ctrl+C”or click“Stop/Restart backend”to exit the
program.

![](/media/d79dc606fd1e2ab55b51822fb5adb5e4.png)

6.  **Wiring Diagram2：**

Control the motor with the S8550（PNP）triode

![](/media/3c3bfe5083b9b963b78e76c3b8d387db.png)

![](/media/08150e9b22904b62ff4b841a8551fbb6.png)

8.  **Test Code 2：**

Go to the folder KS3026 Keyestudio Raspberry Pi Pico Learning Kit Basic
Edition\\2. Windows System\\1. Python\_Tutorial\\2. Python
Projects\\Project 17：Small Fan.

You can move the code to anywhere, for example, we can save the code in
the Disk(D), the route is D:\\2. Python Projects.

Open“Thonny”and click“This computer”→“D:”→“2. Python Projects”→“Project
17: Small Fan”. And double-click“Project\_17.2\_ Small\_Fan.py”

![](/media/af7e516a78e1cb0d6c5318954019f8ed.png)

<table>
<tbody>
<tr class="odd">
<td><p>from machine import Pin</p>
<p>import time</p>
<p>motor = Pin(22, Pin.OUT) # create S8550 object from Pin 22, Set Pin 22 to output</p>
<p>try:</p>
<p>while True:</p>
<p>motor.value(0) # Set motor turn on</p>
<p>time.sleep(4) # Sleep 4s</p>
<p>motor.value(1) # Set motoe turn off</p>
<p>time.sleep(2) # Sleep 2s</p>
<p>except:</p>
<p>pass</p></td>
</tr>
</tbody>
</table>

**Test Result 2：**

Ensure that the Raspberry Pi Pico is connected to the
computer，click“![](/media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](/media/acd099b78a9276a3f77ba78d53cfe732.png)

Click“![](/media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts
executing, we will see that The small fan turns for 5 seconds and stops
for 2 seconds. Press“Ctrl+C”or click“Stop/Restart backend”to exit the
program.

![](/media/3e2cb8a37e5525bfa433c3ca2e457d4a.png)
