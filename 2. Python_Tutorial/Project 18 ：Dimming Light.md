# Project 18: Dimming Light

1.  **Introduction**

A potentiometer is a three-terminal resistor with a sliding or rotating
contact that forms an adjustable voltage divider. It works by varying
the position of a sliding contact across a uniform resistance. In a
potentiometer, the entire input voltage is applied across the whole
length of the resistor, and the output voltage is the voltage drop
between the fixed and sliding contact.

In this project, we are going to learn how to use Raspberry Pi Pico to
read the values of the potentiometer, and make a dimming lamp with LEDs.

2.  **Components Required**

|                                                         |                                      |                          |                             |
| ------------------------------------------------------- | ------------------------------------ | ------------------------ | --------------------------- |
| ![](/media/ef77f5a64c382157fc2dea21ec373fef.png) |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 | Potentiometer\*1         | Red LED\*1                  |
| ![](/media/7dcbd02995be3c142b2f97df7f7c03ce.png)      |
| Breadboard\*1                                           | 220ΩResistor\*1                      | Jumper Wires             | USB Cable\*1                |

3.  **Component Knowledge**
    
    ![](/media/03ab81e8b4f09287d2781ef0fd297f85.png)

**Adjustable potentiometer:** It is a kind of resistor and an analog
electronic component, which has two states of 0 and 1(high level and low
level). The analog quantity is different, its data state presents a
linear state such as 1 \~ 1024.

4.  **Read the Potentiometer Value**
    
    We connect the adjustable potentiometer to the analog IO of the
    Raspberry Pi Pico to read its value and voltage value . Please refer
    to the following wiring diagram for wiring.

![](/media/b8ee6320bce8729a4309857f257d30ec.png)

![](/media/cb970a340d830569e9ac4462a1318e44.png)

The code used in this project is saved in the file KS3026 Keyestudio
Raspberry Pi Pico Learning Kit Basic Edition\\2. Windows System\\1.
Python\_Tutorial\\2. Python Projects\\Project 18：Dimming Light. You can
move the code to anywhere, for example, we can save the code in the
Disk(D), the route is D:\\2. Python Projects.

Open“Thonny, click“This computer”→“D:”→“2. Python Projects”→“Project
18：Dimming Light”. And double left-click
the“Project\_18.1\_Read\_Potentiometer\_Analog\_Value.py”.

![](/media/b1fcd50c4db0ae1272b9b875f8003090.png)

<table>
<tbody>
<tr class="odd">
<td><p>from machine import ADC, Pin</p>
<p>import time</p>
<p># Initialize the potentiometer to pin 26 (ADC function)</p>
<p>adc = ADC(26)</p>
<p># Print the current adc value of the potentiometer cyclically</p>
<p># Print the current voltage value of the potentiometer cyclically</p>
<p>try:</p>
<p>while True:</p>
<p>adcValue = adc.read_u16() # read the ADC value of potentiometer</p>
<p>voltage = adcValue / 65535.0 * 3.3</p>
<p>print("ADC Value:", adcValue, "Voltage:", voltage, "V")</p>
<p>time.sleep(0.1)</p>
<p>except:</p>
<p>pass</p></td>
</tr>
</tbody>
</table>

Ensure that the Raspberry Pi Pico is connected to the
computer，click“Stop/Restart backend”.

![](/media/d7c9612533e1f601716f368cacca3586.png)

Click“Run current script”, the code starts executing, we will see that
the "Shell" window of Thonny IDE will print the ADC value and voltage
value of the potentiomete, turn the potentiometer handle, the ADC value
and voltage value will change. Press“Ctrl+C”or click“Stop/Restart
backend”to exit the program.

![](/media/97f026e8fb8db1d28dd757e35c059d02.png)

![](/media/969b9de3cf505f05d6a9361286cef9c9.png)

5.  **Circuit Diagram and Wiring Diagram**

In the last step, we read the value of the potentiometer, and now we
need to convert the value of the potentiometer into the brightness of
the LED to make a lamp that can adjust the brightness. The wiring
diagram is as follows:

![](/media/66f721b77035d40556c873e0c4577b4a.png)

![](/media/93b03f3cdc8af506d9035b748839ac33.png)

6.  **Test Result**

The code used in this project is saved in the file KS3025 Keyestudio
Raspberry Pi Pico Learning Kit Complete Edition\\2. Windows System\\1.
Python\_Tutorial\\2. Python Projects\\Project 18：Dimming Light. You can
move the code to anywhere, for example, we can save the code in the
Disk(D), the route is D:\\2. Python Projects.

Open“Thonny”, click“This computer”→“D:”→“2. Python Projects”→“Project
18：Dimming Light”. And double left-click
the“Project\_18.2\_Dimming\_Light.py”.

![](/media/308d874689ff5bf3cca0019a7b1bcf1f.png)

<table>
<tbody>
<tr class="odd">
<td><p>from machine import ADC, Pin, PWM</p>
<p>import time</p>
<p>adc = ADC(26) # Initialize the potentiometer to pin 26 (ADC function)</p>
<p>pwm = PWM(Pin(16)) # Initialize the led's PWM to pin 16</p>
<p>pwm.freq(1000) # Define the PWM frequency as 1000</p>
<p>try:</p>
<p>while True:</p>
<p>adcValue = adc.read_u16() # read the ADC value of potentiometer</p>
<p>pwm.duty_u16(adcValue) #map it to the duty cycle of PWM to control led brightness</p>
<p>time.sleep(0.1)</p>
<p>except:</p>
<p>pwm.deinit()</p></td>
</tr>
</tbody>
</table>

7.  **Test Result**
    
    Ensure that the Raspberry Pi Pico is connected to the
    computer，click“Stop/Restart backend”.
    
    ![](/media/6cf698bbc9ffac00f1e474eb554dde1d.png)
    
    Click “Run current script”, the code starts executing, we will see
    that turn the potentiometer handle and the brightness of the LED
    will change accordingly. Press“Ctrl+C”or click“Stop/Restart
    backend”to exit the program.
    
    ![](/media/0bb12cb7c5842d8fbbd5d6d4684ad59e.png)
    
    ![](/media/eca30dead3f4923afa0dcb0306db2319.jpeg)

#
