# **Python_Tutorial(Windows)**

## 1. Preparation for Python:

### 1.1. Install Thonny

Thonny is a free and open source software platform with small size, simple interface, simple operation and rich functions. It is a Python IDE suitable for beginners. In this tutorial, we use this IDE to develop a Raspberry Pi Pico. Thonny supports multiple operating systems including Windows, Mac OS, Linux. 

#### 1.1.1. Download Thonny

1). Enter the website：[https://thonny.org](https://thonny.org) to download the latest version of Thonny.

2). Thonny open-source code library：[https://github.com/thonny/thonny](https://github.com/thonny/thonny).

<table class="colwidths-auto docutils align-default">
<tbody>
<tr class="odd">
<td>System</td>
<td>Download link</td>
</tr>
<tr class="even">
<td>MAC OS：</td>
<td><a href="https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.pkg">https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.pkg</a></td>
</tr>
<tr class="odd">
<td>Windows：</td>
<td><a href=" https:/github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.exe">https://github.com/thonny/thonny/releases/download/v3.2.7/thonny-3.2.7.exe</a></td>
</tr>
<tr class="even">
<td>Linux：</td>
<td><p>Latest version:</p>
<p><strong>Binary bundle for PC (Thonny+Python):</strong></p>
<p>bash &lt;(wget -O - https://thonny.org/installer-for-linux)</p>
<p><strong>With pip:</strong></p>
<p>pip3 install thonny</p>
<p><strong>Distro packages (may not be the latest version):</strong></p>
<p><strong>Debian, Rasbian, Ubuntu, Mint and others:</strong></p>
<p>sudo apt install thonny</p>
<p><strong>Fedora:</strong></p>
<p>sudo dnf install thonny</p></td>
</tr>
</tbody>
</table>


![](./media/bd5823ede2c01d1fa4696438c62aec51.png)

#### 1.1.2. Install Thonny on Windows

1). The downloaded Thonny icon is as follows.

![](./media/d3caa98d406fa06a124d5c98195b90db.png)

2). Double-click “**Thonny-3.3.13.exe**”. The following dialog box is displayed. I choose“![](./media/11fb59a50abe0bf54df7e4cb891ad2c0.png)”to operate. You can also select“![](./media/37be3f3bcc9aa0eb48c8b844eb46a71c.png)” to operate.
    
![](./media/4c044b255da8b14fe674eb9cce01627d.png)
    
3). If you are not familiar with computer software installation, click “**Next**” until the installation is complete.  
    
![](./media/995b36640124b6a9b23f10473ff8a38a.png)
    
![](./media/8bcc17840b9fc15d76f79fee8a0168ee.png)
    
4). If you want to change the route of installing Thonny，just click“**Browse...**” to select a new route and click “**OK**”. 
    
If you don’t want to change the route of installing Thonny, just click “**Next**”and then click “**Next**” again.
    
![](./media/df6f63b42ebb1676b22c26b25dc9c7aa.png)
    
![](./media/f5cd6d619b4645601c5b098ffdbec12a.png)
    
5). Select "**Create Desktop Icon**". Thonny software will generate a shortcut on your desktop for you to open Thonny software later.
    
![](./media/a30c89dde3de81ad00aced30510071be.png)
    
6). Click "**Install**".
    
![](./media/6ace65142291e5e8af5f81e4a6b2f180.png)

7). Wait for a while but don’t click **Cancel**.
    
![](./media/a504b3a3ab16b4d91040cd5878acea0c.png)

8). Once we see the following screen, Thonny software has been successfully installed. Click “**Finish**”.  
    
![](./media/a1fb6027e54a975de1c0aa1e1a0d6a29.png)
    
9). If we select “**Create Desktop Icon**” during the installation, the following icon will be displayed on the desktop.  
    
![](./media/80f35044d91d66f734e36059db35f273.png)

#### 1.1.3. Basic configuration of Thonny software

1). Double-click the desktop icon of Thonny software, we can see the following interface, and we can also choose the language and initial settings.  Once set, click "**Let's Go\!**"  
    
![](./media/ee240978a4f844184f1ea9f5a21d0395.png)
    
![](./media/619a856895d95e00beed748b1438072d.png)
    
![](./media/bcf6c31e4f69c904a7a0c0e9df7e8d7d.png)
    
2). Select “**View**” → “**File**” and “**Shell**”.
    
![](./media/5ff5c305585dbe7e832cc41183db5818.png)
    
![](./media/d41b79772c9846fd8bf295c8451f8321.png)
    
![](./media/3d04fe6893ca104e4e593a0786cb3799.png)

### 1.2. Update Micropython firmware

To run MicroPython programs on Raspberry Pi Pico, we first need to burn a firmware into Raspberry Pi Pico.  

**Why do we need to update the firmware?**

The Raspberry Pi Pico can be programmed in both C and MicroPython, and which is shipped without MicroPython firmware, which we need to download before we can program with MicroPython. 

<span style="color: rgb(255, 76, 65);">Note:</span> MicroPython Firmware only needs to be downloaded once and does not need to be downloaded again when programming with MicroPython.  If we have downloaded the.uf2 firmware written in C, it will be overwritten, so the next time we use MicroPython, we need to update our Raspberry Pi Pico firmware by following the steps.  

#### 1.2.1. Download the Micropython Firmware

**Method 1:** Raspberry Pi Pico official website：[https://www.raspberrypi.com/documentation/microcontrollers/](https://www.raspberrypi.com/documentation/microcontrollers/)

Click the link above, we can see the following interface:

![](./media/3b3e6a639416b76c44f2a0854dc451cc.png)

Scroll the mouse and we can see the following again:

![](./media/5d04d67506852588d126ce760739a3c5.png)

Click MicroPython(Getting Started MicroPython) to go to the firmware download page.  

![](./media/137e21851df02502fb989d8541fa0da8.png)

**Method 2:** By clicking on the download link: [https://micropython.org/download/rp2-pico/rp2-pico-latest.uf2](https://micropython.org/download/rp2-pico/rp2-pico-latest.uf2), we can download directly.  

**Method 3:** If we can't download it due to network problems or other reasons, we can use the.uf2 file we prepared, which is located in the following file path.  

![](./media/ca4858fd34bc267a5b6089ad8ef1d277.png)

#### 1.2.2. Procedures for burning MicroPython firmware

① Connect one end of the microUSB cable to the USB port of our computer.  

② Long press the white button on the "Raspberry Pi Pico" (BOOTSEL).  The Raspberry Pi Pico is then connected to the computer via the microUSB wire.  

![](./media/33c91d51b2aeb2c943691706354aaad1.png)

③ Release the button, when the connection is successful, open \[Device Manager\] on our computer, the computer will automatically recognize the removable disk (RPI-RP2), as shown below:

![](./media/87e24af3ea812b5492a06b0141060b86.png)

④ Copy the file (RP2-Pico-20210902-v1.17.uf2) to a removable disk (RPI-rp2) and wait for it to complete, just like copying the file to a USBflash drive.  

![](./media/916dc807eb08231d8410603e944d405e.png)

⑤ Raspberry Pi Pico automatically restarts after the firmware is burned.  After that, we  can run Micropython.  

### 1.3. Thonny connects to Raspberry Pi Pico

1). Open Thonny, click “Run” and select “Select interpreter…”.

![](./media/09593c45eabe111d9f75848e39312b75.png)

2). Select “Micropython (generic)” or “Micropython (Raspberry Pi Pico)” How to select “Micropython(generic)” ? As follows:

![](./media/0dda06df90ad37a0490c56559108ba51.png)

Select USB-Serial (COMx). The COMx number may be different on different PCS.  Just make sure we select "USB-Serial (COMx)".  

**How to determine which port does the Raspberry Pi Pico communicate with our computer?**

**Step 1:** When our Raspberry Pi Pico is not connected to the computer, open Thonny software, click "Run", select "Select Interpreter", the dialog will pop up, click "Port", we can view the currently connected port, as shown in the picture below:  

![](./media/0112f6cc9da283b3e257d3b1e494f610.png)

**Step 2:** Close the dialog box.  Connect Raspberry Pi Pico to our computer, click "Run" again and select "Select Interpreter".  Click “Port” in the window that is displayed to view the current port.  Now add another port, so this port is used to communicate with the computer.

![](./media/58613bc6727537a24a253c1cc7d9b5cf.jpeg)

**Step 3:** Select “Micropython(generic)” and port, and click“OK”.

![](./media/52262cb23cd963079c41b6b015a43261.jpeg)

**Step 4:** When the following message is displayed on Thonny, then the Thonny successfully connects to the Raspberry Pi Pico.  

![](./media/e33d2e9552d2cecedc50bf96a5036845.png)

So far, all the preparations have been made.

### 1.4. Text Code

**Test Shell Commands:**  

In “**Shell**” window , type “**print (Hello World\!)**”，press “**Enter**”.

![](./media/2b4feabe1126134057046b6a0dd5bbdb.png)

#### 1.4.1. Run Code Online:

To run Raspberry Pi Pico online, we need to connect the Raspberry Pi Pico to our computer, which allows us to compile or debug programs using Thonny software.  

<span style="color: rgb(255, 76, 65);">Advantages:</span> you can compile or debug programs using Thonny software.


Through the "Shell" window, we can view the error information and output results generated during the operation of the program, and query related function information online to help improve the program.  

<span style="color: rgb(255, 76, 65);">Disadvantages:</span> To run Raspberry Pi Pico online, you must connect Raspberry Pi Pico to a computer and run it with Thonny software.  

If the Raspberry Pi Pico is disconnected from the computer, when they reconnect, the program won't run again.  

**Basic Operations:**

Open Thonny and click![](./media/6388aa0daa514f9325fb07fd5ab6749b.png)“**Open...**”.

![](./media/b65264767d6ff04d5f3530b8eebe218c.png)

Click “**This computer**” in the new pop-up window:

![](./media/5bdbc66ef89b41a53e46696c07b2c282.png)

In the new dialog box, go to the folder ...\Python_Codes(Windows)\\Project 01：Hello World . Select “Project\_01\_HelloWorld.py” , click“Open”. The code used in this tutorial is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

![](./media/9b61f563870ec1235e6cc48ca748cec5.png)

Click![](./media/f79b2c42507d12b91ca23ea0bb87c5c2.png) “Run current script” to execute program “Hello World\!”, "Welcome Keyestudio" will print in the “Shell” window.

![](./media/39eb24657c5733544944dd643640a61d.png)

**Exit online**

When running online, click ![Img](./media/img-20231114093533.png) “**Stop /Restart Backend**” on Thonny or press **“Ctrl+C”** to exit the program.  

![](./media/dc2a210535724a7d601b5ad8b02ca8ed.png)

#### 1.4.2. Offline running code:

When running offline, the Raspberry Pi Pico doesn't need to connect to a computer and Thonny.  Once powered up, it can run the main.pyprogram stored in the Raspberry Pi Pico.  

**Pros**: We don't need to connect a computer to Thonny's software to run the program.  

**Cons**: The program stops automatically when an error occurs or the Raspberry Pi Pico runs out of power, and the code is hard to change.

**Basic Operations:** 

Once powered up, the Raspberry Pi Pico will  check for the presence of main\.py on the device automatically.  If so, run the program in main\.py and go to the shell command system.  (If we want the code to run offline, we can save it as main\.py);  If the main\.py does not exist, go directly to the shell command system.  

Click “**File**” → “**New**”, create and write code.

![](./media/7a6988dfff80ecb0479e3e878ccde171.png)

Enter the code in the newly opened file. Here we use the Project\_02\_Onboard\_LED\_Flashing. Py code as an example.  

![](./media/59f397a5c32e3bbe1bb8ff5e2d0316ae.png)

Click“**Save**”on the menu bar, we can save the code in This computer or MicroPython device.

![](./media/abec708857f37ac0871ffa7ad5b4c913.png)

Select “**MicroPython device**”，enter “**main\.py**” in the new pop-up window and click “**OK**”.

![](./media/eb375d7b67d432efb0253a825d5ee5a4.png)

![](./media/d7f40a82158a71b22909f519a9078e94.png)

We can see the code has been uploaded to the Raspberry Pi Pico.

![](./media/aace831a6a8e1199b2a9e0fc6ef40d56.png)

Disconnect the microUSB cable to the Raspberry Pi Pico and reconnect, and the LEDs on the Raspberry Pi Pico will flash repeatedly. 

![Img](./media/img-20231114092907.png)

**Exit Offline**

Connect Raspberry Pi Pico to the computer，click ![Img](./media/img-20231114093514.png) “Stop/Restart backend”on Thonny to end the offline operation.  

![](./media/5efb6f20a190d482be423126eced88d5.png)

If it does’t work, click ![Img](./media/img-20231114093609.png) “Stop/Restart backend”on Thonny several times or reconnect to the Raspberry Pi Pico.

![](./media/0fcf5fad96f698e90f81e37ac5057d80.jpeg)

We provide a main\.py file to run offline.  The code added to main\.py is the bootstrap that executes the user code file. We just need to upload the offline project's code file (<span style="color: rgb(255, 76, 65);">.py</span>) to the "**MicroPython Device**".

Make the program folder **...\6.Codes\Python_Codes(Windows)** move ahead to the Disk(D)，<span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.. Open the Thonny software.  

![](./media/2da93159095ee2355449a27a22f988b4.png)

Expand Project 00 : main in Disk(D) directory D:\\2. Python Projects. Double-click **main\.py** to make the code in "**MicroPython Device**" run offline.  

 ![](./media/30ed08309a2c6d6b53ea9b1cd4beb299.png)

Here, we use project 00 and Project 02 cases as examples. The results are displayed using an LED(GP25 pin) on a Raspberry Pi Pico. If we have modified the Project\_02\_Onboard\_LED\_Flashing. py file, then we need to modify it accordingly. Right-click the Project\_02\_Onboard\_LED\_Flashing. Py file and select '**Upload to/**' to upload the code to Raspberry Pi Pico, as shown below.  

![](./media/2b0dfdd7becf42730b1baa0ca45e6ea3.png)

Upload the **main\.py** in the same way.

![](./media/4e8bc42dbffa1e0432a94e99977d426f.jpeg)

Disconnect and reconnect the microUSB cable to the Raspberry Pi Pico, and the LEDs will flash repeatedly .

![Img](./media/img-20231114092857.png)

<span style="color: rgb(255, 76, 65);">Note:</span>

The code here runs offline.  If we want to stop running offline and go to "**Shell**", simply click ![Img](./media/img-20231114093459.png) "Stop/Restart Backend" on Thonny software.

![](./media/dc2a210535724a7d601b5ad8b02ca8ed.png)

### 1.5. Thonny Common Operations:

#### Upload the code to Raspberry Pi Pico:

In the Project 01：Hello World file, right-click and select Project\_01\_HelloWorld.py，select“**Upload to /**”and upload the code to the root directory of the Raspberry Pi Pico.

![](./media/18f24b958cc2efe1e332c429383b8df1.png)

#### Download the code to the computer:

In the “**MicroPython device**”, right-click and select Project\_01\_HelloWorld.py，select “**Download to ...**” to download the code to our computer.

![](./media/867e40f907c512aa4a17c0f4fb6d75e6.png)

#### Delete the files in the Raspberry Pi Pico root directory:

In the “**MicroPython device**”, right-click and select Project\_01\_HelloWorld.py, select “**Delete**”, delete the Project\_01\_HelloWorld.py from the Raspberry Pi Pico root directory.

![](./media/d97823ab15b1afd831a438e2863ab270.png)

#### Delete files from the computer's directory:

In the Project\_01 : Hello World file, right-click and select Project\_01\_HelloWorld.py, select “**Move to Recycle Bin**”, then it can be deleted from the Project\_01\_HelloWorld file.

![](./media/9d73a385a0855eb68c453088bd0748f4.png)

#### Create and Save Code:

① Click “**File**” → “**New**” to create and compile code.

![](./media/373922a344188cda87b797b0ad639522.png)

② Enter code in the newly opened file, here we use Project\_02\_Onboard\_LED\_Flashing.py code as an example.

![](./media/4aab2202442af7b04e880414af8f44fe.png)

③ Click “**Save**”, and we can save the code to our computer or the Raspberry Pi Pico.

![](./media/19773e65bc454d549ae95422b645692a.png)

④ Select “**MicroPython device**”, enter “**main\.py**” in the new pop-up window and click “**OK**”.

![](./media/92c1b5f2bb76f21462da37cdb9a3f18f.png)

![](./media/d7f40a82158a71b22909f519a9078e94.png)

⑤ We can see the code has been uploaded to the Raspberry Pi Pico.

![](./media/4be452d7471f5110efdc50737007d714.png)

⑥ Click “**Run current script**”, the LED on the Raspberry Pi Pico will flash periodically.

![](./media/3c0b64be3cc1a0750f187e063dcabd29.png)

![Img](./media/img-20231114092857.png)


## 2. Projects：

When we get the kit, we can see that there are some sensors, modules and electronic components in the kit, which contain the corresponding Raspberry Pi Pico mainboard, Raspberry Pi Pico Expansion Board and wirings. 

<span style="color: rgb(255, 76, 65);">Note: </span>When connecting the electronic components, modules, sensor wirings in the projects, the wiring method and position must be followed in the document. What’s more, do not misconnect the power supply and signal pin, otherwise there may be no experimental results or damage to the modules/sensors. 

### Project 01: Hello World

#### 1. Introduction:

For Raspberry Pi Pico beginners, we will start with some simple things. In this project, you only need a Raspberry Pi Pico and a USB cable to complete the "Hello World\!" project, which is a test of communication between Raspberry Pi Pico and the PC as well as a primary project.

#### 2. Components:

| ![2e2bec86b3985dab2f1c07dfdb89ba73](media/2e2bec86b3985dab2f1c07dfdb89ba73.jpeg) |![](media/3bdcc62cfa661d2b860a76e28537e21e.png)|
| ------------------------------- | ---------------------- |
| Raspberry Pi Pico\*1            | USB Cable\*1           |

#### 3. Wiring Up:

In this project, we use a USB cable to connect the Raspberry Pi Pico to the computer.

![](./media/8ea81d60b8e2132c358041235490b7d5.jpeg)

#### 4. Online running code:

To run the Raspberry Pi Pico online, you need to connect the Raspberry Pi Pico to your computer, which allows you to compile or debug programs using Thonny software.  

**Advantages:**

1)\. You can use the Thonny software to compile or debug programs.

2)\. Through the "Shell" window, you can view error messages and output results generated during the running of the program as well as query related function information online to help improve the program.  

**Disadvantages**:

1)\. To run the Raspberry Pi Pico online, you must connect the Raspberry Pi Pico to a computer and run it with the Thonny software.  

2)\. If the Raspberry Pi Pico is disconnected from the computer, when they reconnect, the program won't run again.  

**Basic Operation:**

1)\. Open Thonny and click “Open...”.

![](./media/b65264767d6ff04d5f3530b8eebe218c.png)

2)\. Click“This computer”in the new pop-up window.

![](./media/5bdbc66ef89b41a53e46696c07b2c282.png)

In the new dialog box, select “Project\_01\_HelloWorld.py”, click “Open”.

The code used in this tutorial is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

![](./media/9b61f563870ec1235e6cc48ca748cec5.png)

3)\. Click “![](./media/f79b2c42507d12b91ca23ea0bb87c5c2.png)Run current script” to execute the program “Hello World\!”, "Welcome Keyestudio", which will be printed in the “Shell” window.

![](./media/39eb24657c5733544944dd643640a61d.png)

#### 5. Exit running online:

When running online, click![](./media/fee1916cdaf53677f5117fbc5b65f4cf.png)“Stop /Restart Backend” or press “Ctrl+C” to exit the program.  

![](./media/dc2a210535724a7d601b5ad8b02ca8ed.png)

#### 6. Text Code:

```python
print("Hello World!")
print("Welcome Keyestudio")
```

### Project 02: Onboard LED flashing

#### 1. Introduction:

Raspberry Pi Pico has an onboard LED, which is a GP25 pin attached to the Raspberry Pi Pico. In this project, we will learn the effect of making the onboard LED blink. 

#### 2. Components:

| ![2e2bec86b3985dab2f1c07dfdb89ba73](media/2e2bec86b3985dab2f1c07dfdb89ba73-16853475831642.jpeg) |![](media/3bdcc62cfa661d2b860a76e28537e21e-16853475768291.png)|
| ------------------------------- | ---------------------- |
| Raspberry Pi Pico\*1            | USB Cable\*1           |

#### 3. Wiring Up:

In this project, we use a USB cable to connect the Raspberry Pi Pico to the computer. Please refer to the documentation for the connection methods: Preparation for Python（Important）

![](./media/8ea81d60b8e2132c358041235490b7d5.jpeg)

#### 4. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

**Code running online:**

Open “Thonny” ，click “This computer” → “D:” → “Python_Codes(Windows)” →“Project 02：Onboard LED flashing”.

![](./media/17519952e7c0019f1f0591903caa26d8.png)

Enter the file “Project 02：Onboard LED flashing”，double left-click the file “Project\_02\_Onboard\_LED\_flashing.py”, open it, as follows:

![](./media/87a877076f95cbe7d684ecc05de3e0cf.png)

```python
from machine import Pin
import time

led = Pin(25, Pin.OUT)   # create LED object from Pin 25, Set Pin 25 to output

try:
    while True:
        led.value(1)    # Set led turn on
        time.sleep(0.5) # Sleep 0.5s
        led.value(0)    # Set led turn off
        time.sleep(0.5) # Sleep 0.5s
except:
    pass
```


Ensure that the Raspberry Pi Pico is connected to the computer, click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”，then see what the **"Shell**" window displays.

![](./media/a53cb17aaa0b29d1c5f359f222868c69.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts to execute, we will see that the LED on the Raspberry Pi Pico begins flashing. Press “Ctrl+C”or click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/79796116d54281366ee2e4871dd4ca33.png)

![Img](./media/img-20231114092857.png)

<span style="color: rgb(255, 76, 65);">Note:</span> This is the code that runs online.  If you disconnect the USB cable and restart the Raspberry Pi Pico, the LEDS on the Raspberry Pi Pico will stop flashing. The following information will be displayed in the "Shell" window of Thonny software:  

![](./media/dde0b82feb441565c2bfa9517dedfed0.png)

**Code running offline**（upload the code to the Raspberry Pi Pico）：

Ensure that the Raspberry Pi Pico is connected to the computer, click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/705d3bdd9cad821399137c7c0df72e86.png)

As shown in the following figure, right-click the file “Project\_02\_Onboard\_LED\_flashing.py” and select “**Upload to /**” to upload the code to the Raspberry Pi Pico.  

![](./media/4e83ee98b0da014fae6896f4fb14c889.png)

Upload main\.py in the same way.

![](./media/1591c6146bbcd2df9c9ba1aec14a86ca.png)

Disconnect the USB cable from the Raspberry Pi Pico and reconnect, and the LED will flash repeatedly. 

![Img](./media/img-20231114092857.png)

<span style="color: rgb(255, 76, 65);">Note:</span> The code here runs offline.  If you want to stop it and display the information in the "Shell" window, simply click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) "Stop/Restart Backend" in Thonny software.  

![](./media/f7ca5b1be220957141fb119e6cc4ab37.png)



### Project 03：External LED flashing

#### 1. Introduction:

In this project, we are going to show you the external LED flashing effect.  We will use the Raspberry Pi Pico's digital pins to turn on the LED and make it flash.

#### 2. Components:

| ![2e2bec86b3985dab2f1c07dfdb89ba73](media/2e2bec86b3985dab2f1c07dfdb89ba73-16853479111433.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9.png) | ![](media/wps73.png) |![3ec5906fad2172708d449390140f55e6](media/3ec5906fad2172708d449390140f55e6.png)|
| ------------------------------------------------------- | ------------------------------------ | ---------------------- | ---------------------- |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 | Breadboard\*1 | Red LED\*1 |
| ![image-20230529161414632](media/image-20230529161414632.png) |![](media/7dcbd02995be3c142b2f97df7f7c03ce.png)|![c801a7baee258ff7f5f28ac6e9a7097b](media/c801a7baee258ff7f5f28ac6e9a7097b.png)| |
| 220Ω Resistor\*1                                             | USB Cable\*1                                    | Jumper Wire\*2         |            |

#### 3. Knowledge:

**（1）LED:**

![3ec5906fad2172708d449390140f55e6](media/3ec5906fad2172708d449390140f55e6.png)

The LED is a kind of semiconductor called “light-emitting diode”, which is an electronic device made from semiconducting materials (silicon, selenium, germanium, etc.).  It has a anode and a cathode.  The short lead is cathode, which connects to GND, the long lead is anode , which connects to3.3V or 5V.

![](./media/f70404aa49540fd7aecae944c7c01f83.jpeg)

**（2）5-band Resistor**

A resistor is an electronic component in a circuit that restricts or regulates the flow current flow. On the left is the appearance of the resistor and on the right is the symbol for the resistance in the circuit . Its unit is(Ω). 1 mΩ= 1000 kΩ，1kΩ= 1000Ω.

![image-20230529161535645](media/image-20230529161535645.png)

We can use resistors to protect sensitive components, such as LEDs. The strength of the resistance is marked on the body of the resistor with an electronic color code. Each color code represents a number, and you can refer to it in a resistance card.

![](./media/c3df005312cd9f6d4cdae6abf3cddb83.png)

In this kit, we provide three 5-band resistors with different resistance values. Take three 5-band resistors as an example.

220Ω resistor\*10

![](./media/55c0199544e9819328f6d5778f10d7d0.png)

10KΩ resistor\*10

![](./media/246cf3885dc837c458a28123885c9f7b.png)

1KΩ resistor\*10

![](./media/19f5dfc51adfd79b04c3b164529767ed.png)

In the same voltage, there will be less current and more resistance. The connection between current, voltage, and resistance can be expressed by the formula: I=U/R. In the figure below, if the voltage is 3V, the current through R1 is: I = U / R = 3 V / 10 KΩ= 0.0003A= 0.3mA.

![](./media/b3eec552e4dfad361833730698621776.png)

Do not directly connect resistors with very low resistance to the two poles of the power supply, as this will cause excessive current to damage the electronic components. Resistors do not have positive and negative poles.

**（3）Breadboard**

A breadboard is used to build and test circuits quickly before finalizing any circuit design. The breadboard has many holes , into which circuit components like integrated circuits and resistors can be inserted. A typical breadboard is as follows.

![](./media/612c1381811b2d780d5f6ed6a7ec3701.png)

The bread board has strips of metal , which run underneath the board and connect the holes on the top of the board. The metal strips are laid out as shown below. Note that the top and bottom rows of holes are connected horizontally while the remaining holes are connected vertically.

![](./media/b45e70b961537035c85878b73d371725.png)

The first two rows (top) and the last two rows (bottom) of the breadboard are used for the positive (+) and negative (-) terminals of the power supply, respectively. The conductive layout of the breadboard is shown in the following diagram.

![](./media/d5478bd5eac558252cbc235479d979eb.png)

When we connect DIP (Dual In-line Packages) components, such as integrated circuits, microcontrollers, chips and so on, we can see that a groove in the middle isolates the middle part, so the top and bottom of the groove is not connected. DIP components can be connected as shown in the figure below:

![](./media/50caf14e911c4244779e99445c658db6.png)

![](./media/9b66ae2199e77fbc99b7b278dac0b567.png)

#### 4. How to use the keyestudio raspberry pico expansion board:

Stack the Raspberry Pi Pico on the expansionboardto use, as shown below:


![](./media/fae969ca3b1a4592a83a4e05f5795a5b.png)

#### 5. Power Supply:

In this project, we use a USB to connect the Raspberry Pi Pico to the computer. Please refer to the documentation for connection methods: Preparation for Python

![](./media/8ea81d60b8e2132c358041235490b7d5.jpeg)

#### 6. Circuit Diagram and Wiring Diagram:

First, cut all power to the Raspberry Pi Pico. Then build the circuit according to the circuit diagram and wiring diagram.  After the circuits are set up and verified, using a USB cable to connect the Raspberry Pi Pico to a computer .  Note: Avoid any possible short circuits (especially connecting 3.3V and GND)\!

<span style="color: rgb(255, 76, 65);">Warning:</span> A short circuit may cause a large current in the circuit, causing components to overheat and permanent damage to the hardware.

![](./media/cb069d7553d861e3293d8bdbe85bbd05.png)

**Circuit Diagram:**

![](./media/898285da10fa9b39e52a02bc68758d27.png)

**Wiring Diagram:**

Note:

How to connect a LED

![](./media/42ff6f405dfa128593827de5aa03e94b.png)

How to identify the 220Ω five-band resistor

![](./media/55c0199544e9819328f6d5778f10d7d0.png)

#### 7. Test Code:

According to the circuit diagram, when the GP16 output of the Pico is high, the LED will light up;  When the output power is low, the LED will light off.  Therefore, we can make the LED flash repeatedly by controlling the GP16 to repeatedly output high and low levels.  

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

**Code running online:**

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 03：External LED flashing”.

![](./media/4607246406f23fa569aa3cea202f3863.png)

Enter the file “Project 03: External LED flashing”, double left-click  “Project\_03\_External\_LED\_flashing.py”, open it, as shown below:

![](./media/387934a09c74f4d5c0e8ed19c4cde926.png)

```python
from machine import Pin
import time

led = Pin(16, Pin.OUT)   # create LED object from Pin 16, Set Pin 16 to output

try:
    while True:
        led.value(1)    # Set led turn on
        time.sleep(0.5) # Sleep 0.5s
        led.value(0)    # Set led turn off
        time.sleep(0.5) # Sleep 0.5s
except:
    pass
```


Ensure that the Raspberry Pi Pico is connected to the computer, click “![fee1916cdaf53677f5117fbc5b65f4cf](media/fee1916cdaf53677f5117fbc5b65f4cf.png)Stop/Restart backend” and see what will display in the “Shell” window.

![](./media/139fa290786502af65584b20ba61fb82.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts to execute, and the LED will begin flashing. Press “Ctrl+C” or click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/f0a8b15499b9ef17c9d09002aafa4d58.png)

![image-20230529162737631](media/image-20230529162737631.png)

<span style="color: rgb(255, 76, 65);">Note:</span> This is the code that runs online, if we disconnect the USB cable, then restart the“Raspberry Pi Pico”, the LED will stop flashing. The following information will be displayed in the "Shell" window of Thonny software:  

<br>
<br>

![](./media/20f0f44738c9119895ccbf2dadb21a65.png)

**Code running offline**（Upload the code to the Raspberry Pi Pico）：

Ensure that the Raspberry Pi Pico is connected to the computer, click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”

![](./media/6a9f8cdac46a55b5e0f3d8ba4ee6f0f9.png)

As shown below, right-click the file “Project\_03\_External\_LED\_flashing.py”，select “**Upload to /**” to upload the code to the Raspberry Pi Pico.

![](./media/60ed038ee245d8c58cd921d388988b81.png)

Upload **main\.py** in the same way.

![](./media/6ab80f86d06be94d54bd5c737370151d.png)

Disconnect the USB from the Raspberry Pi Pico and reconnect, the LED in the circuit will flash repeatedly.

![image-20230529162737631](media/image-20230529162737631.png)

<span style="color: rgb(255, 76, 65);">Note:</span> The code here runs offline.  If you want to stop and display the information in the Shell window, simply click“Stop/Restart backend” in Thonny software.  

![](./media/f7ca5b1be220957141fb119e6cc4ab37.png)


### Project 04: Breathing Led

#### 1. Introduction:

In previous studies, we know that LEDS have on/off state, so how to enter the intermediate state?  That's what we're going to learn.  Breathing lights, or LEDS turn on and off again, which are like "breathing". So, how to control the brightness of LEDS?  We will use the Raspberry Pi Pico PWM to achieve this goal.  

#### 2. Components:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) | ![](media/wps73.png) |![afa6edd3ff90b027a6f43995a6fb15a2](media/afa6edd3ff90b027a6f43995a6fb15a2.png)|
| ------------------------------------------------------- | ------------------------------------ | ---------------------- | ---------------------- |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 | Breadboard\*1 | Red LED\*1 |
| ![](./media/7dcbd02995be3c142b2f97df7f7c03ce.png) |![image-20230529163514816](media/image-20230529163514816.png)|![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png)| |
| USB Cable\*1                                                 | 220Ω Resistor\*1                     | Jumper Wire\*2         |            |

#### 3. Knowledge:

![](./media/6549bdbfd4e7b6b2b341012105d655e8.png)

**Analog & Digital**

Analog signals are continuous signals in both time and value.  In contrast, a digital or discrete time signal is a time series consisting of a series of numbers.  Most signals in life are analog signals.  

A familiar example of an analog signal is how temperatures change continuously throughout the day, rather than suddenly changing from 0 to 10 in a flash.  However, the value of a digital signal can change instantaneously. This change is represented numerically as 1 and 0(the basis of binary code).  It's easier to see the difference, as shown below:

![](./media/4bdf6127e563b453a1fd8953b4ebb277.png)

In practical applications, we often use a binary as a digital signal, which are a series of 0 and 1. Since binary signals have only two values (0 or 1), they have great stability and reliability.  Finally, analog and digital signals can be converted to each other. 

**PWM：**

Pulse Width Modulation (PWM) is an effective method to control analog circuit by digital signal. Ordinary processors cannot directly output analog signals. The PWM makes this conversion (convert digital signal to analog signal) very convenient, which uses digital pins to send square waves at a certain frequency, which is high and low output to alternate for a period of time. The total time of each set of high and low levels is generally fixed, which is called the period (Note: the reciprocal of the period is the frequency). The time of the high level output is usually called pulse width, and the duty cycle is the percentage of the pulse width (PW) to the total period (T) of the waveform. The longer the duration of the high level output as well as the duty cycle is, the higher the corresponding voltage in the analog signal will be. The figure below shows the variation of analog signal voltage from 0V to 3.3V(high level is 3.3V) corresponding to pulse width of 0% to 100%.  

![](./media/a439e1bd8a4578b43b7188c821d58594.jpeg)

We all know that the longer the PWM duty cycle is, the higher the output power will be. Therefore, we can use PWM to control the brightness of LEDS or the speed of dc motors and so on.  As can be seen from the above, the PWM is not a real analog signal, and the effective value of the voltage is equal to the corresponding analog signal.  Therefore, we can control the output power of LEDS and other output modules to achieve different effects.

**Raspberry Pi Pico and PWM**

The Raspberry Pi Pico has 16 PWM channels, each of which can control frequency and duty cycle independently. The clock frequency ranges from 7Hz to 125MHz.  Each pin on the Raspberry Pi Pico can be configured for PWM output.  

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/cb069d7553d861e3293d8bdbe85bbd05.png)

![](./media/898285da10fa9b39e52a02bc68758d27.png)

**Note:**

How to connect the LED

![](./media/42ff6f405dfa128593827de5aa03e94b.png)

How to identify the 220Ω 5-band resistor

![](./media/55c0199544e9819328f6d5778f10d7d0.png)

#### 5. Test Code:

The design of this project makes the GP16 output PWM, and the pulse width gradually increases from 0% to 100%, and then gradually decreases from 100% to 0%.  

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 04：Breathing Led”. And double left-click “Project_04_Breathing_Led.py”.

![](./media/d0616993fc8b1deb9db4414e3146e602.png)

```python
#MicroPython implementation of raspberry PI Pico board LED breathing lamp program example
import time
from machine import Pin,PWM
PWM_PulseWidth=0
#Using external LED, build PWM object PWM LED
pwm_LED=PWM(Pin(16))
#Set the PWM LED frequency
pwm_LED.freq(500)
while True:
    while PWM_PulseWidth<65535:
        PWM_PulseWidth=PWM_PulseWidth+50
        time.sleep_ms(1)   #Delay 1 ms 
        pwm_LED.duty_u16(PWM_PulseWidth)
    while PWM_PulseWidth>0:
        PWM_PulseWidth=PWM_PulseWidth-50
        time.sleep_ms(1)
        pwm_LED.duty_u16(PWM_PulseWidth)
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, and click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/4daa8b74aec8af6056ec2a61ebabf397.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts to execute, we will see that The LEDS in the circuit fade from dark to light, and then from light to dark again, which is like breathing . Press“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Ctrl+C”or“Stop/Restart backend”to exit the program.

![](./media/957f4e2178c1126f724bc8e012568e31.png)

![image-20230529163728017](media/image-20230529163728017.png)


### Project 05：Traffic Lights

#### 1. Introduction:

Traffic lights are closely related to people's daily lives, which generally show red, yellow, and green. Everyone should obey the traffic rules, which can avoid many traffic accidents. In this project, we will use Raspberry Pi Pico and some LEDs (red, green and yellow) to simulate the traffic lights.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) |![](media/wps73.png) |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi Pico Expansion Board*1                          | Breadboard*1                                                 |
| ![afa6edd3ff90b027a6f43995a6fb15a2](media/afa6edd3ff90b027a6f43995a6fb15a2.png) | ![0c1b0f91b4e56bcbc235d06b48809ac9](media/0c1b0f91b4e56bcbc235d06b48809ac9.png) | ![6c688493b558ed5f3e90e7dab38cbd93](media/6c688493b558ed5f3e90e7dab38cbd93.png) |
| Red LED*1                                                    | Yellow LED*1                                                 | Green LED*1                                                  |
| ![](media/7dcbd02995be3c142b2f97df7f7c03ce-168534956642710.png) | ![image-20230529163514816](media/image-20230529163514816.png) | ![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png) |
| USB Cable*1                                                  | 220ΩResistor*3                                               | Jumper Wires                                                 |

#### 3. Circuit Diagram and Wiring Diagram:

![](./media/4cf2ad735b0df82d62a5fcdb19ebf3c0.png)

![](./media/98f9db025163638c33095cbd16abe7e7.png)

Note:

How to connect an LED

![](./media/42ff6f405dfa128593827de5aa03e94b.png)

How to identify the 220Ω 5-band resistor

![](./media/55c0199544e9819328f6d5778f10d7d0.png)

#### 4. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → ”Project 05：Traffic Lights”and double left-click the “Project\_05\_Traffic\_Lights.py”.

![](./media/23e79112920bc111a9bc621dc75162a0.png)

```python
from machine import Pin
import time

led_red = machine.Pin(16, machine.Pin.OUT)  # create red led object from Pin 16, Set Pin 16 to output
led_yellow = machine.Pin(17, machine.Pin.OUT)  # create yellow led object from Pin 17, Set Pin 17 to output
led_green = machine.Pin(18, machine.Pin.OUT) # create green led object from Pin 18, Set Pin 18 to output

while True:
    led_red.value(1)  # Set red led turn on
    time.sleep(5)   # Sleep 5s
    led_red.value(0) # Set red led turn off 
    led_yellow.value(1)
    time.sleep(0.5)
    led_yellow.value(0)
    time.sleep(0.5)
    led_yellow.value(1)
    time.sleep(0.5)
    led_yellow.value(0)
    time.sleep(0.5)
    led_yellow.value(1)
    time.sleep(0.5)
    led_yellow.value(0)
    time.sleep(0.5)
    led_green.value(1)
    time.sleep(5) 
    led_green.value(0) 
```

#### 5. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/914349b7c46f99b24beaada57db00815.png)

Click“![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts executing, what we will see are below:

1). First, the green light will be on for 5 seconds and then off; 

2). Next, the yellow light blinks three times and then goes off. 

3). Then, the red light goes on for five seconds and then goes off. 
    

Repeat steps 1 to 3 above and press“Ctrl+C”or click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/ff8674d60cc99a8c3bbef24bf65ae20c.png)


### Project 06: RGB LED

#### 1. Introduction:

![](./media/94bdff69e438989d8e0934e57f2e5c00.png)

RGB LEDS are made up of three colors (red, green, and blue) , which can emit different colors by mixing these three basic colors. In this project, we will introduce the RGB LED and show you how to use the Raspberry Pi Pico to control the RGB LED. Even though RGB LED is very basic, it is also a great way to learn the fundamentals of electronics and coding.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) |![](media/f1a86fc81ab4b043263ce7e01e14d470.png)|![](media/wps73.png)|
| ------------------------------------------------------- | ------------------------------------ | ------------------------------- | ---------------------- |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 | RGB LED\*1                      | Breadboard\*1 |
| ![image-20230529163514816](media/image-20230529163514816.png) |![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce-168534973856512.png)| |
| 220ΩResistor\*3                                         | Jumper Wires                                                 | USB Cable\*1                                                 |                                                              |

#### 3. Component Knowledge:

The monitors mostly adopt the RGB color standard, and all the colors on the computer screen are composed of the three colors of red, green and blue mixed in different proportions.

![](./media/8bf1339719a922f2fbc1e01a4347b4ab.png)

This RGB LED has 4 pins and a common cathode. To change its brightness, we can use the PWM of the Raspberry Pi Pico pins, which can give different duty cycle signals to the RGB LED to produce different colors.

If we use three 10-bit PWM to control the RGBLED, theoretically we can create ![Img](./media/img-20231115112655.png) = 1,073,741,824(1 billion) colors through different combinations.

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/f6950bc8498e6139cbb67db84cdd5a9a.png)

![](./media/fdab8c2fd2dfdd1670c09962e7b458ce.png)

**Note:**

RGB LED longest pin (common cathode) connected to GND.

![](./media/1584356c63bf99934ae0810ee02dced3.png)

How to identify the 220Ω 5-band resistor

![](./media/55c0199544e9819328f6d5778f10d7d0.png)

#### 5. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” →“D:” → “Python_Codes(Windows)” → “Project 06：RGB LED”. And double left-click the “Project\_06\_RGB\_LED.py”.

![](./media/4d197d2ef390d93cbdcd6606fa754188.png)

```python
# import Pin, PWM and Random function modules.
from machine import Pin, PWM
from random import randint
import time

#configure ouput mode of GP18, GP17 and GP16 as PWM output and PWM frequency as 10000Hz.
pins = [18, 17, 16]
freq_num = 10000

pwm0 = PWM(Pin(pins[0]))  #set PWM
pwm1 = PWM(Pin(pins[1]))
pwm2 = PWM(Pin(pins[2]))
pwm0.freq(freq_num)
pwm1.freq(freq_num)
pwm2.freq(freq_num)

#define a function to set the color of RGBLED.
def setColor(r, g, b):
    pwm0.duty_u16(65535 - r)
    pwm1.duty_u16(65535 - g)
    pwm2.duty_u16(65535 - b)
    
try:
    while True:
        red   = randint(0, 65535) 
        green = randint(0, 65535)
        blue  = randint(0, 65535)
        setColor(red, green, blue)
        time.sleep_ms(200)
except:
    pwm0.deinit()
    pwm1.deinit()
    pwm2.deinit() 
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/a2b85aea8a2bd67ad184662be36a1c9e.png)

Click ![](./media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code startsexecuting, we will see that RGB LED starts showing random colors. Press“Ctrl+C”or click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”to exit the program.

![](./media/296bcab9a2eaccf483b8cb9e8b8a0e43.png)


### Project 07: Flowing Water Light

#### 1. Introduction:

In our daily life, we can see many billboards made up of different colors of LED. They constantly change the light to attract the attention of customers. 

In this project, we will use Raspberry Pi Pico to control 10 LEDs to achieve the effect of flowing water.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) | ![](media/wps73.png)| ![3ec5906fad2172708d449390140f55e6](media/3ec5906fad2172708d449390140f55e6.png) |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi Pico Expansion Board*1                          | Breadboard*1                                                 | Red LED*10                                                   |
| ![image-20230529163514816](media/image-20230529163514816.png) | ![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png) | ![](media/7dcbd02995be3c142b2f97df7f7c03ce-168534973856512.png) |                                                              |
| 220ΩResistor*10                                              | Jumper Wires                                                 | USB Cable*1                                                  |                                                              |

#### 3. Circuit Diagram and Wiring Diagram:

![](./media/e6f92039d131685369db2d1ac2c30267.png)

![](./media/fc6e73a6664012c9a33262b50d6e256f.png)

**Note:**

How to connect the LED

![](./media/42ff6f405dfa128593827de5aa03e94b.png)

How to identify the 220Ω 5-band resistor

![](./media/55c0199544e9819328f6d5778f10d7d0.png)

#### 4. Test Code:

This project is to design and manufacture a flowing water light. Here are the steps: first , turn on LED #1, then turn it off. Second, turn on LED #2, then turn off... . Do the same for the 10 LEDs until the last one is turned off. Repeating the process to achieve the "movement" of the water.

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 07：Flowing Water Light”. And double left-click the “Project_07_Flowing_Water_Light.py”.

![](./media/a923fafe77f629ea8288ec40b52a6059.png)

```python
from machine import Pin
import time

#Use an array to define 10 GPIO ports connected to LED Bar Graph for easier operation.
pins = [16, 17, 18, 19, 20, 21, 22, 26, 27, 28]
#Use two for loops to turn on LEDs separately from left to right and then back from right to left
def showLed():
    for pin in pins:
        print(pin)
        led = Pin(pin, Pin.OUT)
        led.value(1)
        time.sleep_ms(100)
        led.value(0)
        time.sleep_ms(100)        
    for pin in reversed(pins):
        print(pin)
        led = Pin(pin, Pin.OUT)
        led.value(1)
        time.sleep_ms(100)
        led.value(0)
        time.sleep_ms(100)
          
while True:
    showLed()
```

#### 5. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/b908750521d4d2b64c55751825916a7e.png)

Click ![](./media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, we will see that the 10 LEDs will light up from left to right and then return from right to left. Press “Ctrl+C”or click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”to exit the program.

![](./media/c9814fae261b7f8c9d2b33938d8e6144.png)

![image-20230529164842179](media/image-20230529164842179.png)


### Project 08: 1-Digit Digital Tube

#### 1. Introduction:

The seven-segment digital tube is an electronic display device that displays decimal numbers. It is widely used in digital clocks, electronic meters, basic calculators and other electronic devices that display digital information. The tubes are an alternative to more complex dot-matrix displays that are easy to use in both limited light conditions and strong sunlight. In this project, we will use the Raspberry Pi Pico to control 1-digit digital tube to display numbers.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) | ![75e38d601750a4707369bc73d8028063](media/75e38d601750a4707369bc73d8028063.png) | ![](media/wps73.png)|
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi Pico Expansion Board*1                          | 1-digit Digital Tube*1                                       | Breadboard*1                                                 |
| ![image-20230529163514816](media/image-20230529163514816.png) | ![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png) | ![](media/7dcbd02995be3c142b2f97df7f7c03ce-168534973856512.png) |                                                              |
| 220ΩResistor*8                                               | Breadboard Wires                                             | USB Cable*1                                                  |                                                              |

#### 3. Component Knowledge:

![](./media/e44a0f27beec739ee13e68c04865989f.png)

**Display principle:** 

The digital tube display is a semiconductor light-emitting device.  Its basic unit is a light-emitting diode (LED). The digital tube display can be divided into 7-segment digital tube and 8-segment digital tube according to the number of segments. The 8-segment digital tube has one more LED unit than the 7-segment digital tube (used for decimal point display). Each segment of the 7-segment LED display is a separate LED. According to the connection mode of the LED unit, the digital tube can be divided into a common anode digital tube and a common cathode digital tube.

In the common cathode 7-segment digital tube, all the cathodes (or negative electrodes) of the segmented LEDs are connected together, so you should connect the common cathode to GND. To light up a segmented LED, you can set its associated pin to“HIGH”.

In the common anode 7-segment digital tube, the LED anodes (positive electrodes) of all segments are connected together, so you should connect the common anode to “+5V”. To light up a segmented LED, you can set its associated pin to “LOW”.

![](./media/28fd057848fbe0e8c8e3362768e7aa44.png)

Each part of the digital tube is composed of an LED. So when you use it, you also need to use a current limiting resistor. Otherwise, the LED will be damaged. In this experiment, we use an ordinary common cathode one-bit digital tube. As we mentioned above, you should connect the common cathode to GND. To light up a segmented LED, you can set its associated pin to “HIGH”.

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/84e67e0ce2d7627a96b83156324d92d5.png)

**Note:** 

The direction of the 7-segment digital tube inserted into the breadboard is the same as the wiring diagram, and there is one more point in the lower right corner.

![](./media/66da2f88234019c4a712494174ea4426.png)

![](./media/d99daa4165cf32b2283aae82466981bd.png)

#### 5. Test Code:

The digital display is divided into 7 segments, and the decimal point display is divided into 1 segment. When certain numbers are displayed, the corresponding segment will be illuminated. For example, when the number 1 is displayed, segments b and c will be opened.

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 08：1-Digit Digital Tube”. And double left-click the  “Project_08_One_Digit_Digital_Tube.py”.

![](./media/c9b3cf2f06c5261b112afde681d7c3a2.png)

```python
from machine import Pin
import time

a = machine.Pin(17, machine.Pin.OUT)
b = machine.Pin(16, machine.Pin.OUT)
c = machine.Pin(14, machine.Pin.OUT)
d = machine.Pin(13, machine.Pin.OUT)
e = machine.Pin(12, machine.Pin.OUT)
f = machine.Pin(18, machine.Pin.OUT)
g = machine.Pin(19, machine.Pin.OUT)
dp = machine.Pin(15, machine.Pin.OUT)

pins = [machine.Pin(id,machine.Pin.OUT) for id in [17, 16, 14, 13, 12, 18, 19, 15]]

def show(code):
    for i in range(0, 8):
        pins[i].value(~code & 1)
        code = code >> 1

#Select code from 0 to 9
mask_digits = [0xc0, 0xf9, 0xa4, 0xb0, 0x99, 0x92, 0x82, 0xf8,0x80, 0x90]
for code in reversed(mask_digits):
    show(code)
    time.sleep(1)
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/f6eed549d1acfd058333e95306edeb1d.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script” , the code starts executing, we will see that the 1-digit digital tube will display numbers from 9 to 0. Press “Ctrl+C” or click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/4d06038bf94823da20012d28475cc6b9.png)


### Project 09：4-Digit Digital Tube

#### 1. Introduction:

The 4-digit 7-segment digital tube is a very practical display device, and it is used for devices such as electronic clocks and score counters. Due to the low price and it is easy to use, more and more projects will use 4-digit 7-segment digital tubes. In this project, we will use the Raspberry Pi Pico to control a 4-bit 7-segment digital tube to create a manual counter.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) | ![85cfe0f4b888f5543316d1eebbfde4f8](media/85cfe0f4b888f5543316d1eebbfde4f8.png) | ![](media/wps73.png)|
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi Pico Expansion Board*1                          | 4-Digit Digital Tube Module*1                                | Breadboard*1                                                 |
| ![image-20230529163514816](media/image-20230529163514816.png) | ![](media/7dcbd02995be3c142b2f97df7f7c03ce-168534973856512.png) | ![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png) |                                                              |
| 220Ω Resistor*8                                              | USB Cable*1                                                  | Jumper Wires                                                 |                                                              |

#### 3. Component Knowledge:

![](./media/ce987bf9a2ab398945c98b34d3f8a003.png)

**4-digital tube display:**

The 4-digital tube display is is a semiconductor light-emitting device.  Its basic unit is a light-emitting diode (LED). The digital tube display can be divided into 7-segment digital tube and 8-segment digital tube according to the number of segments. The 8-segment digital tube has one more LED unit than the 7-segment digital tube (used for decimal point display). Each segment of the 7-segment LED display is a separate LED. According to the connection mode of the LED unit, the digital tube can be divided into a common anode digital tube and a common cathode digital tube.

In the common cathode 7-segment digital tube, all the cathodes (or negative electrodes) of the segmented LEDs are connected together, so you should connect the common cathode to GND. To light up a segmented LED, you can set its associated pin to“HIGH”.

Pins of control bit are G1, G2, G3 and G4.

![](./media/37113fa53213973132086c285d67686b.png)

![](./media/ea75d1b7414bf6f8c187fb32fea9bc83.png)

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/4f64b9bf6b74ab49584f69c7465efa73.png)

![](./media/6bf1bae6af0324d50a37ab7a0cabee11.png)

#### 5. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 09：4-Digit Digital Tube”. And double left-click the “Project_09_Four_Digit_Digital_Tube.py”.

![](./media/e30515a97d87169cc191a0c9775b78b2.png)

```python
from machine import Pin
import time

#Pin of each digit of nixie tube
a = machine.Pin(21, machine.Pin.OUT)
b = machine.Pin(28, machine.Pin.OUT)
c = machine.Pin(16, machine.Pin.OUT)
d = machine.Pin(18, machine.Pin.OUT)
e = machine.Pin(19, machine.Pin.OUT)
f = machine.Pin(22, machine.Pin.OUT)
g = machine.Pin(15, machine.Pin.OUT)
dp = machine.Pin(17, machine.Pin.OUT)

G1 = machine.Pin(20, machine.Pin.OUT)
G2 = machine.Pin(26, machine.Pin.OUT)
G3 = machine.Pin(27, machine.Pin.OUT)
G4 = machine.Pin(14, machine.Pin.OUT)
 
#digital tube a to dp corresponding development board pins
d_Pins=[machine.Pin(i,machine.Pin.OUT)  for i in [21,28,16,18,19,22,15,17]]
#Pin corresponding to digital tube segment G1, G2, G3, and G4
w_Pins=[machine.Pin(i,machine.Pin.OUT)  for i in [20,26,27,14]]
 
number={
    '0':
    [1,1,1,1,1,1,0,0],#0
    '1':
    [0,1,1,0,0,0,0,0],#1
    '2':
    [1,1,0,1,1,0,1,0],#2
    '3':
    [1,1,1,1,0,0,1,0],#3
    '4':
    [0,1,1,0,0,1,1,0],#4
    '5':
    [1,0,1,1,0,1,1,0],#5
    '6':
    [1,0,1,1,1,1,1,0],#6
    '7':
    [1,1,1,0,0,0,0,0],#7
    '8':
    [1,1,1,1,1,1,1,0],#8
    '9':
    [1,1,1,1,0,1,1,0],#9
}
 
def display(num,dp):
    global number
    count=0
    for pin in d_Pins:#displays the value of num 
        pin.value(number[num][count])
        count+=1
    if dp==1:
        d_Pins[7].value(0)
def clear():
    for i in w_Pins:
        i.value(0)
    for i in d_Pins:
        i.value(1)
def showData(num):
   #the hundreds, thousands, ones, and fractional values of a numeric value
    d_num=num
    location=d_num.find('.')
    if location>0:
        d_num=d_num.replace('.','')
        while len(d_num)<4:
            d_num='0'+d_num
        for i in range(0,4):
            time.sleep(2)
            clear()
            w_Pins[3-i].value(1)
            if i==location-1:
                display(d_num[i],1)
            else:
                display(d_num[i],0)
    if location<0:
        for i in range(0,4):
            time.sleep(2)
            clear()
            w_Pins[3-i].value(1)
            display(d_num[i],0)
while True:
 
    num='9016'
showData(num)
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer，click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/682029610c29b14122b37787bbd2ae53.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts executing, we will see that the 4-digit digital tube circularly displays numbers from 0000 to 9999. Press “Ctrl+C” or click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/3ef28f4dda60e7c14e1ffd8aa5d823aa.png)


### Project 10：8×8 Dot-matrix Display

#### 1. Introduction:

The dot-matrix display is an electronic digital display device that can show information on machines, clocks and many other devices. In this project, we will use the Raspberry Pi Pico to control the 8x8 LED dot matrix to make a “❤” pattern.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) | ![d226a1f3c801ac78321f0692143c853e](media/d226a1f3c801ac78321f0692143c853e.png) | ![](media/wps73.png)|
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi Pico Expansion Board*1                          | 8*8 Dot-matrix Display *1                                    | Breadboard*1                                                 |
| ![image-20230529163514816](media/image-20230529163514816.png) | ![b1991d0d88442db1d6b2f4189530397b](media/b1991d0d88442db1d6b2f4189530397b.png) | ![](media/7dcbd02995be3c142b2f97df7f7c03ce-168534973856512.png) |                                                              |
| 220Ω Resistor*8                                              | M-F Dupont Wires                                             | USB Cable*1                                                  |                                                              |

#### 3. Component Knowledge:

**8\*8 Dot-matrix display module:**

The 8x8 dot matrix is composed of 64 LEDs, and each LED is placed at the intersection of a row and a column. When using a single-chip microcomputer to drive an 8x8 dot matrix, we need to use a total of 16 digital ports, which greatly wastes the data of the single-chip microcomputer. For this reason, we specially designed this module, using the HT16K33 chip to drive an 8x8 dot matrix, and only need to use the I2C communication port of the single-chip microcomputer to control the dot matrix, which greatly saves the microcontroller resources.

![](./media/69c719a7898907ab32f089f0cbbaff13.png)

![](./media/bcfa2498367eaf9c7733da15af32eae7.png)

#### 4. Schematic diagram:

![](./media/094a47e28b2c735ab475ede10c0deb43.png)

#### 5. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 10：8×8 Dot-matrix Display”. And double-click the “Project_10_8×8_Dot_Matrix_Display.py”.

![](./media/33278d3cbc3b0cb185963a1d5e50e209.png)

```python
from machine import Pin
import time

#Define the pin of the row and Set to output
row1 = machine.Pin(18, machine.Pin.OUT)
row2 = machine.Pin(26, machine.Pin.OUT)
row3 = machine.Pin(17, machine.Pin.OUT)
row4 = machine.Pin(21, machine.Pin.OUT)
row5 = machine.Pin(10, machine.Pin.OUT)
row6 = machine.Pin(16, machine.Pin.OUT)
row7 = machine.Pin(11, machine.Pin.OUT)
row8 = machine.Pin(14, machine.Pin.OUT)
#Define the pins of the column and Set to output
col1 = machine.Pin(22, machine.Pin.OUT)
col2 = machine.Pin(12, machine.Pin.OUT)
col3 = machine.Pin(13, machine.Pin.OUT)
col4 = machine.Pin(19, machine.Pin.OUT)
col5 = machine.Pin(15, machine.Pin.OUT)
col6 = machine.Pin(20, machine.Pin.OUT)
col7 = machine.Pin(27, machine.Pin.OUT)
col8 = machine.Pin(28, machine.Pin.OUT)

#Sets the pin of the column to low level
col1.value(0)
col2.value(0)
col3.value(0)
col4.value(0)
col5.value(0)
col6.value(0)
col7.value(0)
col8.value(0)

#Since the column of the lattice has been set to low level, the corresponding row of the lattice will light up when the pin of the row is at high level
def Row(d):
    if(d ==1):
        row1.value(1)  #Light the first line
    if(d ==2):
        row2.value(1)  #Light the second line
    if(d ==3):
        row3.value(1)
    if(d ==4):
        row4.value(1)
    if(d ==5):
        row5.value(1)
    if(d ==6):
        row6.value(1)
    if(d ==7):
        row7.value(1)
    if(d ==8):
        row8.value(1)
    
#Close the lattice
def off():
    row1.value(0)
    row2.value(0)
    row3.value(0)
    row4.value(0)
    row5.value(0)
    row6.value(0)
    row7.value(0)
    row8.value(0) 

try:
    print("test...")
    while True:
         for num in range(1,10):  #Light the lattice line by line
             Row(num)
             if(num == 9):  #Because the lattice has only 8 rows, and I'm limiting it here, is equal to 9
                off()      #Close the lattice
             time.sleep(0.2)

except:
    pass
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend”.

![](./media/d195d37e4eb32c656c741c8c6c391572.png)

Click ![](./media/da852227207616ccd9aff28f19e02690.png) “Run current script”, the code starts executing, we will see that the 8 x 8 dot matrix displays the character "A" 1S, "B" 1S, and "C" 1S. Then scroll to display the string "Hello World”repeatedly. Press “Ctrl+C”or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/476f84b2194fc6ef6e9d2df0cbd787d4.png)

### Project 11：74HC595N Control 8 LEDs 

#### 1. Introduction:

In previous projects, we have learned how to light an LED.  However, how to light up a lot of LEDs with only 26 I/O ports on the Raspberry Pi Pico? Sometimes we may run out of pins , at that time, we need to extend it with the shift register. You can use a 74HC595N chip to control up to eight outputs at a time, using only a few pins on your microcontroller. In addition, You can also connect multiple registers together to further expand the output. In this project, we will use a Raspberry Pi Pico, a 74HC595 chip and LEDs to make a flowing water light to understand the function of the chip.  

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) |![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png)| ![](media/6921c6d60135e072ed4bd24564ec4a6d.png) |![](media/3ec5906fad2172708d449390140f55e6-168535106780428.png)|
| ------------------------------------------------------- | ------------------------------------ | ---------------------- | --------------------------- |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 | 74HC595N Chip\*1 | Red LED\*8                  |
| ![image-20230529163514816](media/image-20230529163514816.png) |![](media/wps73.png)|![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce-168535107138729.png)|
| 220ΩResistor\*8                                         | Breadboard\*1                        | Jumper Wires                                    | USB Cable\*1                |

#### 3. Component Knowledge:

![](./media/6921c6d60135e072ed4bd24564ec4a6d.png)

**74HC595N Chip:** 

To put it simply, 74HC595N chip is a combination of 8-digit shifting register, memorizer and equipped with tri-state output. The shift register and the memorizer are synchronized to different clocks, and the data is input on the rising edge of the shift register clock SCK and goes into the memory register on the rising edge of the memory register clock RCK. If the two clocks are connected together, the shift register is always one pulse earlier than the storage register. The shift register has a serial shift input (SI) and a serial output (SQH) for cascading. The 8-bit shift register can be reset asynchronously (low-level reset), and the storage register has an 8-bit Three-state parallel bus output, when the output enable (OE) is enabled (active low), the storage register is output to the 74HC595N pin (bus).

![](./media/858b189f06ad68afe051b15043b2affd.png)

| PIN                   | FUNCION                                                      |
| --------------------- | ------------------------------------------------------------ |
| Pin13 OE              | It is an output enable pin to ensure that the data of the latch is input to the Q0 to Q7 pins or not. When it is low, no high level is output. In this experiment, we directly connect to GND and keep the data output low. |
| Pin14 SI              | This is the pin for 74HC595 to receive data, i.e. serial data input, only one bit can be input at a time, then 8 times in a row, it can form a byte. |
| Pin10 SCLR            | A pin to initialize the storage register pins. It initializes the internal storage registers at a low level. In this experiment, we connect VCC to maintain a high level. |
| Pin11 SCK             | The clock pin of the shift register. At the rising edge, the data in the shift register is shifted backward as a whole, and new data input is received. |
| Pin12 RCK             | The clock input pin of the storage register . At the rising edge, the data is transferred from the shift register to the storage register. At this time, the data is output in parallel from the Q0 to Q7 ports. |
| Pin9 SQH              | It is a serial output pin dedicated for chip cascading to the SI terminal of the next 74HC595. |
| Q0--Q7(Pin 15,Pin1-7) | Eight-bit parallel output, can directly control the 8 segments of the digital tube. |

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/1738cecf584c83b55370153ebc1688b7.png)

Note: Pay attention to the direction in which the 74HC595N chip is inserted.

![](./media/a6d03617539b70d6d69fa7e9acb25be9.png)

![](./media/91833532723f4ee623902c0252092741.png)

#### 5. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 11：74HC595N Control 8 LEDs”. Select “my74HC595\.py”， right-click and select “**Upload to /**”，wait for “my74HC595\.py” to be uploaded to the Raspberry Pi Pico. And double left-click the “Project_11_74HC595N_Controls_8_LEDs.py”.

![](./media/e062ee8e0d8ac1aaba4df1ff403d3cf3.png)

![](./media/2325da1459f6092c063eac913e620264.png)

```python
#Import time and my74HC595 modules.
from my74HC595 import Chip74HC595
import time

#Create a Chip74HC595 object and configure pins
chip = Chip74HC595(18, 20, 21)
#Chip74HC595() == Chip74HC595(18, 20, 21)

#The first for loop makes LED Bar display separately from left to rightwhile the second for loop make it display separately from right to left.
while True:
    x = 0x01
    for count in range(8):
        chip.shiftOut(1, x)
        x = x<<1;
        time.sleep_ms(300)
    x = 0x01
    for count in range(8):
        chip.shiftOut(0, x)
        x = x<<1
        time.sleep_ms(300)
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer，click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend”.

![](./media/faebdbd5720409f07bf6c03ee6ba9d65.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts executing, we will see that the 8 LEDs start flashing in flowing water mode. Press “Ctrl+C” or click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/eda98e28568ebec03cc1ec41ec6492b1.png)


###  Project 12：Active Buzzer

#### 1. Introduction:

Active buzzer is a sound making element, which is widely used on computers, printers, alarms, electronic toys, telephones, timers, etc. It has an inner vibration source. In this project, we will use a Raspberry Pi Pico to control the active buzzer to buzz.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) |![](media/wps73.png)|
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi Pico Expansion Board*1                          | Breadboard*1                                                 |
| ![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png) | ![](media/7dcbd02995be3c142b2f97df7f7c03ce-168535107138729.png) | ![4b4f653a76a82a3b413855493cc58fba](media/4b4f653a76a82a3b413855493cc58fba.png) |
| Jumper Wires                                                 | USB Cable*1                                                  | Active Buzzer*1                                              |

#### 3. Component Knowledge:

![](./media/11ec5ddc982db9928341e858aab94652.png)

The active buzzer inside has a simple oscillator circuit , which can convert constant direct current into a certain frequency pulse signal. Once active buzzer receives a high level, it will sound. The passive buzzer is an integrated electronic buzzer with no internal vibration source. It must be driven by 2K to 5K square wave instead of a DC signal. The appearance of the two buzzers is very similar, but passive buzzers come with a green circuit board, and active buzzers come with a black tape. Passive buzzers don't have positive pole, but active buzzers have. As shown below:

![](./media/0f9825969867ac2d65bb1a19ed0ad2ab.png)

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/48e73ef2d6090fe7cda58c385bad2ab2.png)

![](./media/56df73f7ac711e510b30164c5759615f.png)

<span style="color: rgb(255, 76, 65);">Note:</span>

1)\. The buzzer power supply in this circuit is 5V.  On a 3.3V power supply, the buzzer will work, but it will reduce the loudness.  

2)\. The VUSB should connect to the positive terminal of the USB cable, if it connects to GND, it could burn out the computer or Raspberry Pi Pico.  Similarly, the Raspberry Pi Pico's 36-40 pins need to be connected carefully to avoid short circuits. 

3)\. The positive terminal ("+"/long pin) of the active buzzer is connected to pin 16, and the negative terminal (short pin) is connected to GND.

#### 5. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 12：Active Buzzer”. And double left-click the  Project\_12\_Active\_Buzzer.py”.

![](./media/a2b4775a67925f2380686d61ec5e9b71.png)

```python
from machine import Pin
import time

buzzer = Pin(16, Pin.OUT)   # create buzzer object from Pin 16, Set Pin 16 to output

try:
    while True:
        buzzer.value(1)    # Set buzzer turn on
        time.sleep(0.5) # Sleep 0.5s
        buzzer.value(0)    # Set buzzer turn off
        time.sleep(0.5) # Sleep 0.5s
except:
    pass
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, and click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/29ff4d3cfefcc7cef8786a31d004da30.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts executing, we will see that the the active buzzer starts to buzz. Press “Ctrl+C” or click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/655dae76dfb3987d7ed9bc5838711b2e.png)


### Project 13：Passive Buzzer

#### 1. Introduction:

In a previous project, we have learned an active buzzer, which can only produce one sound and may let you feel monotonous. In this project, we will learn a passive buzzer and use the Raspberry Pi Pico to control the passive buzzer to sound an alarm. Unlike the active buzzer, the passive buzzer can emit sounds of different frequencies.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) |![](media/wps73.png) |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi PicoExpansion Board*1                           | Breadboard*1                                                 |
| ![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png) | ![](media/7dcbd02995be3c142b2f97df7f7c03ce-168535107138729.png) | ![5444cd34945d9cc2dbb825a8be8d49ad](media/5444cd34945d9cc2dbb825a8be8d49ad.png) |
| Jumper Wires                                                 | USB Cable*1                                                  | Passive Buzzer*1                                             |

#### 3. Component Knowledge:

![](./media/8d0020e53824072cbe9d4f7d2f8acb4f.png)

A passive buzzer is an integrated electronic buzzer with no internal vibration source. It must be driven by 2K to 5K square wave, not a DC signal. The two buzzers are very similar in appearance, but one buzzer with a green circuit board is a passive buzzer, while the other with black tape is an active buzzer. Passive buzzers cannot distinguish between positive polarity while active buzzers can.

![](./media/fc42c5ed014609ff0b290ee5361bb2fd.png)

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/e0da1ccdbff24d256db130816c55da74.png)

![](./media/e601e48f8deddb3e9e7734d0022106b3.png)

#### 5. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 13：Passive Buzzer”. And double left-click the “Project\_13\_Passive\_Buzzer.py”.

![](./media/4e4cf166f1de082468ebf77ef6ba3d4d.png)

```python
from machine import Pin
import time

#Initialize the passive buzzer
buzzer = Pin(16,Pin.OUT)

#Simulate two different frequencies
while True:
    #Output 500HZ frequency sound
    for i in range(80):
        buzzer.value(1)
        time.sleep(0.001)
        buzzer.value(0)
        time.sleep(0.001)
    #Output 250HZ frequency sound
    for i in range(100):
        buzzer.value(1)
        time.sleep(0.002)
        buzzer.value(0)
        time.sleep(0.002)
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer，click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”.

![](./media/699667c6aea0990e6a2fa408ef7ca3a1.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts executing, we will see that the the passive buzzer sounds the alarm. Press “Ctrl+C” or click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/02d6cb5bd3d2cef4e669886b957544ed.png)


### Project 14 : Mini Table Lamp

#### 1. Introduction:

Did you know that a Raspberry Pi Pico can light up an LED when you press a button? In this project, we will use the Raspberry Pi Pico, a key switch and an LED to make a Mini Table lamp.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) | ![5b8fea4657b47510d199f740fdcaaa9d](media/5b8fea4657b47510d199f740fdcaaa9d.png) | ![](media/wps73.png)|
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi Pico Expansion Board*1                          | Button*1                                                     | Breadboard*1                                                 |
| ![7eb361d680dfa351f07f8527aeb37abd](media/7eb361d680dfa351f07f8527aeb37abd.png) | ![image-20230529171550381](media/image-20230529171550381.png) | ![image-20230529161414632](media/image-20230529161414632.png) | ![8defa4d3994ce0f2291b05c2fd04ee9c](media/8defa4d3994ce0f2291b05c2fd04ee9c.png) |
| Red LED*1                                                    | 10KΩResistor*1                                               | 220ΩResistor*1                                               | Button Cap*1                                                 |
| ![](media/7dcbd02995be3c142b2f97df7f7c03ce-168535107138729.png) | ![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png) |                                                              |                                                              |
| USB Cable*1                                                  | JumperWires                                                  |                                                              |                                                              |

#### 3. Component Knowledge:

![](./media/5b8fea4657b47510d199f740fdcaaa9d.png)

**Button:** 

The button can control the circuit on and off. The circuit is disconnected when the button is not pressed. But it breaks when you release it. Why does it only work when you press it? It starts from the internal structure of the button, which is shown in the figure:![](./media/d2a204e61c768f18924150db58aee093.png). 

Before the button is pressed, 1 and 2 are on, 3 and 4 are also on, but 1, 3 or 1, 4 or 2, 3 or 2, 4 are off (not working). Only when the button is pressed, 1, 3 or 1, 4 or 2, 3 or 2, 4 are on. The key switch is one of the most commonly used components in circuit design.

**Schematic diagram of the button:**

![image-20230529171622424](media/image-20230529171622424.png)

**What is button jitter?**

We think of the switch circuit as "press the button and turn it on immediately", "press it again and turn it off immediately". In fact, this is not the case.

The button usually uses a mechanical elastic switch, and the mechanical elastic switch will produce a series of jitter due to the elastic action at the moment when the mechanical contact is opened and closed (usually about 10ms). As a result, the button switch will not immediately andstably turn on the circuit when it is closed, and it will not be completely and instantaneously disconnected when it is turned off.

![](./media/7e7ac82db8bb810a7ee1de4181ceaa2d.jpeg)

**How to eliminate the jitter?**

There are two common methods, namely fix jitter in the software and hardware. We only discuss the jitter removal in the software.

We already know that the jitter time generated by elasticity is about 10ms, and the delay command can be used to delay the execution time of the command to achieve the effect of jitter removal. Therefore, we delay 0.02s in the code to achieve the key anti-shake function.

![](./media/c0d68d1134b0b4097e8983ed2cac07fc.jpeg)

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/0753a2a452e0292b31f79f9b6dabb0cc.png)

![](./media/a03a6553dc194ab61fb7b4d914740f90.png)

**Note:**

How to connect the LED

![](./media/f70404aa49540fd7aecae944c7c01f83.jpeg)

How to identify the 220Ω 5-band resistor and 10KΩ 5-band resistor

![](./media/55c0199544e9819328f6d5778f10d7d0.png)

![](./media/246cf3885dc837c458a28123885c9f7b.png)

#### 5. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 14：Mini Table Lamp”. And double left-click the “Project\_14\_Mini\_Table\_Lamp.py”.

![](./media/0efc0a37e75cff4ac3d0007dbf3f2829.png)

```python
from machine import Pin
import time

led = Pin(19, Pin.OUT) # create LED object from Pin 19,Set Pin 19 to output                   
button = Pin(22, Pin.IN, Pin.PULL_UP) #Create button object from Pin22,Set GP22 to input

#Customize a function and name it reverseGPIO(),which reverses the output level of the LED
def reverseGPIO():
    if led.value():
        led.value(0)     #Set led turn off
    else:
        led.value(1)     #Set led turn on

try:
    while True:
        if not button.value():
            time.sleep_ms(20)
            if not button.value():
                reverseGPIO()
                while not button.value():
                    time.sleep_ms(20)
except:
    pass
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer，click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/32daa1b963c18ba89686184df6e0ffe9.png)

Click ![](./media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, we will see that press the button, the LED lights up;  when the button is released, the LED remains lit.  Press the button again, the LED goes off;  

When the button is released, the LED remains off. Doesn't it look like a little lamp? Press“Ctrl+C”or click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”to exit the program.

![](./media/f208593b20f934d9b8c71e6e7905cccd.png)


### Project 15：Tilt And LED

#### 1. Introduction:

The ancients without electronic clocks, so the hourglass are invented to measure time.  The hourglass has a large capacity on both sides, and which is filled with fine sand on one side. What’s more, there is a small channel in the middle, which can make the hourglass stand upright , the side with fine sand is on the top. However, due to the action of gravity, the fine sand will flow down through the channel to the other side of the hourglass. When the sand reaches the bottom, turn it upside down and record the number of times it has gone through the hourglass, therefore, the next day we can know the approximate time of the day by it. In this project, we will use a Raspberry Pi Pico to control the tilt switch and LED lights to simulate an hourglass and make an electronic hourglass. 

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) |![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png)|![8c40739f8e05f753f145420b421a0f47](media/8c40739f8e05f753f145420b421a0f47.png)|![7eb361d680dfa351f07f8527aeb37abd](media/7eb361d680dfa351f07f8527aeb37abd.png)|![image-20230529171550381](media/image-20230529171550381.png)|
| ------------------------------------------------------- | ------------------------------------ | ---------------------- | --------------------------- | -------------------------- |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 | Tilt Switch\*1         | Red LED\*4                  | 10KΩResistor\*1            |
| ![](media/wps73.png) | ![image-20230529161414632](media/image-20230529161414632.png) |![](media/7dcbd02995be3c142b2f97df7f7c03ce-168535107138729.png)|![](media/e9a8d050105397bb183512fb4ffdd2f6-168535187611242.png)| |
| Breadboard\*1                                           | 220ΩResistor\*4                      | USB Cable\*1           | Jumper Wires                |                            |

#### 3. Component Knowledge:

![](./media/8c40739f8e05f753f145420b421a0f47.png)

Tilt switch is also called digital switch. Inside is a metal ball that can roll. The principle of rolling the metal ball to contact with the conductive plate at the bottom, which is used to control the on and off of the circuit. When it is a rolling ball tilt sensing switch with single directional trigger, the tilt sensor is tilted toward the trigger end (two gold-plated pin ends), the tilt switch is in a closed circuit and the voltage at the analog port is about 5V (binary number is 1023). In this way, the LED will light up. When the tilt switch is in a horizontal position or tilted to the other end, it is open and the voltage of the analog port is about 0V (binary number is 0), the LED will turn off. In the program, we judge the state of the switch based on whether the voltage value of the analog port is greater than 2.5V (binary number is 512).

As shown in the figure, use the internal structure of the tilt switch to illustrate how it works.

![](./media/bf8b10ad248ac939ac4ef96d02ed87c7.png)

#### 4. Circuit Diagram and Wiring Diagram:

![](./media/8735f9531646b77c35932404a681b76d.png)

![](./media/9127e65ff0d7b3d5e579263fd06ec674.png)

Note:

How to connect the LED

![](./media/f70404aa49540fd7aecae944c7c01f83.jpeg)

How to identify the 220Ω 5-band resistor and 10KΩ 5-band resistor

![](./media/55c0199544e9819328f6d5778f10d7d0.png)

![](./media/246cf3885dc837c458a28123885c9f7b.png)

#### 5. Text Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 15：Tilt And LED”. And double-click the “Project\_15\_Tilt\_And\_LED.py”.

![](./media/f6e58ba03bbfa0cf1707b1e48ae4968d.png)

```python
from machine import Pin
import time

led1 = Pin(19, Pin.OUT) # create LED object from Pin 19,Set Pin 19 to output
led2 = Pin(18, Pin.OUT) # create LED object from Pin 18,Set Pin 18 to output
led3 = Pin(17, Pin.OUT) # create LED object from Pin 17,Set Pin 17 to output
led4 = Pin(16, Pin.OUT) # create LED object from Pin 16,Set Pin 16 to output
Tilt_Sensor = Pin(22,Pin.IN) #Create tilt object from Pin22,Set GP22 to input

while True:
    if(Tilt_Sensor.value() == 0) : #when the value of tilt sensor is 0
        led1.value(1) # led1 turn on
        time.sleep_ms(200)#delay
        led2.value(1) # led2 turn on
        time.sleep_ms(200)#delay
        led3.value(1) # led3 turn on
        time.sleep_ms(200)#delay
        led4.value(1) # led4 turn on
        time.sleep_ms(200)#delay 
    else :           #when the value of tilt sensor is 1
        led4.value(0) # led4 turn off
        time.sleep_ms(200)#delay
        led3.value(0) # led3 turn off
        time.sleep_ms(200)#delay
        led2.value(0) # led2 turn off
        time.sleep_ms(200)#delay
        led1.value(0) # led1 turn off
        time.sleep_ms(200)#delay
```

#### 6. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/d1171ab1ce593168fbe85f0b36ab5a0f.png)

Click ![](./media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, we will see that when you tilt the breadboard to an angle, the LEDs will light up one by one. When you turn the breadboard to the original angle, the LEDs will turn off one by one. Like the hourglass, the sand will leak out over time. Press “Ctrl+C” or click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) Stop/Restart backend” to exit the program.

![](./media/71e2f26ed3dc928a66d9950e8862cfed.png)


### Project 16: I2C 128×32 LCD

#### 1. Introduction:

We can use modules such as monitors to do various experiments in life. You can also DIY a variety of small objects. For example, you can make a temperature meter with a temperature sensor and display, or make a distance meter with an ultrasonic module and display.

In this project, we will use the LCD\_128X32\_DOT module as a display and connect it to a Raspberry Pi Pico, which will be used to control the LCD\_128X32\_DOT display to show various English characters, common symbols and numbers.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) |![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png)|![9232141f8a3166a8a6cdd43b78edd4e3](media/9232141f8a3166a8a6cdd43b78edd4e3.png)|![f1aed48e2c02214415853ad2358f3744](media/f1aed48e2c02214415853ad2358f3744.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce-168535202993546.png)|
| ------------------------------------------------------- | ----------------------- | --------------------------- | ---------------------- |---------------------- |
| Raspberry Pi Pico\*1  |  Raspberry Pi Pico Expansion Board\*1                                 | LCD\_128X32\_DOT\*1     | 10CM M-F Dupont Wires       | USB Cable\*1           |

#### 3. Component Knowledge:

![](./media/2c2645e94a00867ac23e8a022f0a631a.png)

**LCD\_128X32\_DOT:** 

It is an LCD module with 128*32 pixels and its driver chip is ST7567A. The module uses the IIC communication mode, while the code contains a library of all alphabets and common symbols that can be called directly. When using, we can also set it in the code so that the  English letters and symbols show different text sizes. To make it easy to set up the pattern display, we also provide a mold capture software that converts a specific pattern into control code and then copies it directly into the test code for use.

#### 4. Schematic diagram:

![](./media/5451aed32bc5b7b30fbd5613ad09a65b.png)

**Features:**

Pixel: 128\*32 character

Operating voltage(chip)：4.5V to 5.5V

Operating current：100mA (5.0V)

Optimal operating voltage(module):5.0V

#### 5. Circuit Diagram and Wiring Diagram:

Note: The LCD\_128X32\_DOT must be connected with 10CM M-F Dupont wires, which can make the LCD\_128X32\_DOT display normally. Otherwise, using 20CM M-F Dupont wires may cause the LCD\_128X32\_DOT display abnormally.  

![](./media/82aae0a70e5628c53d7f81f7730cf79a.png)

#### 6. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny” , click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 16：I2C 128×32 LCD”. Select “lcd128_32.py” and “lcd128_32_fonts.py”，right-click and select “**Upload to /**”，wait for the “lcd128_32.py” and the “lcd128_32_fonts.py” to be uploaded to the  Raspberry Pi Pico. And double left-click the “Project_16_I2C_128_32_LCD.py”.

![](./media/a5317de4b98628b494bdcb500ea4419e.png)

![](./media/67f8290c36e92a858c41e2655208cd6d.png)

![](./media/2eccc2ce9fc4a29ad3bd8bee67128546.png)

```python
import machine
import time
import lcd128_32_fonts
from lcd128_32 import lcd128_32

#i2c config
clock_pin = 21
data_pin = 20
bus = 0
i2c_addr = 0x3f
use_i2c = True

def scan_for_devices():
    i2c = machine.I2C(bus,sda=machine.Pin(data_pin),scl=machine.Pin(clock_pin))
    devices = i2c.scan()
    if devices:
        for d in devices:
            print(hex(d))
    else:
        print('no i2c devices')

if use_i2c:
    scan_for_devices()
    lcd = lcd128_32(data_pin, clock_pin, bus, i2c_addr)

lcd.Clear()

lcd.Cursor(0, 4)
lcd.Display("KEYESTUDIO")
lcd.Cursor(1, 0)
lcd.Display("ABCDEFGHIJKLMNOPQR")
lcd.Cursor(2, 0)
lcd.Display("123456789+-*/<>=$@")
lcd.Cursor(3, 0)
lcd.Display("%^&(){}:;'|?,.~\\[]")
"""
while True:
    scan_for_devices()
    time.sleep(0.5)
"""
```

#### 7. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer，click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/beb9d64377903a417b29ddf4f8b1bcae.png)

Click“![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts executing, we will see that the LCD module display will show "KEYESTUDIO" at the first line. "ABCDEFGHIJKLMNOPQR" will be displayed at the second line. "123456789 + - \* / \<\> = $ @ " will be shown at the third line and "% ^ & () {} :; '|?,. \~ \\\\ \[\] " will be displayed at the fourth line. Press“Ctrl+C”or click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”to exit the program.

![](./media/4eb4b9cf7ed2b34877a326c0a5251cac.png)


### Project 17：Small Fan

#### 1. Introduction:

In the hot summer, we need an electric fan to cool us down, so in this
project, we will use the Plus control board to control 130 motor module
and small blade to make a small fan.

#### 2. Components Required:

| ![2e2bec86b3985dab2f1c07dfdb89ba73](media/2e2bec86b3985dab2f1c07dfdb89ba73.jpeg) | ![](media/bbed91c0b45fcafc7e7163bfeabf68f9-16854050283871.png) | ![image-20230530080645428](media/image-20230530080645428.png) | ![](media/wps73.png)|
| ------------------------------------------------------- | ------------------------------------ | ---------------------- | ----------------------- |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 | S8550 Triode\*1 | Breadboard\*1                                                |
| ![image-20230530080525691](media/image-20230530080525691.png) | ![image-20230530080537718](media/image-20230530080537718.png) |![](media/9197d4aff9356c585b7ef68e33a6881d.png)| |
| DC Motor\*1                                             | Fan\*1                                                       | S8050 Triode\*1                                              |                                                              |
| ![image-20230530080553619](media/image-20230530080553619.png) |![image-20230530080607415](media/image-20230530080607415.png)|![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce-16854050342952.png)|
| 1KΩ Resistor\*1                                              | Diode\*1                                                     | Jumper Wires           | USB Cable\*1                                                 |

#### 3. Component Knowledge:

![](./media/9197d4aff9356c585b7ef68e33a6881d.png)

**Triode：**

It is referred as the semiconductor triode and a bipolar transistor or a transistor.

The triode is one of the basic semiconductor components as the core of the electronic circuit., which can amplify current. The triode means that two PN junctions are made on a semiconductor wafer. The two PN junctions divide the entire semiconductor into three parts. The middle part is the base area, and the two sides are the emitter and collector areas.

As for NPN triode, it is composed of two N type semiconductors and a P type semiconductor.

The type of transistor which may be used in some applications in place of the triode tube is the "junction" transistor, which actually has two junctions. It has an emitter, base, and collector which correspond to the cathode, grid, and plate, respectively, in the triode tube. Junction transistors are of two types, the NPN type and the PNP type.

The PN junction between the emitting area and the base area is emitter junction and the PN junction flanked by the collector area and the base area is collector junction. And three pins are E（Emitter), B (Base)and C (Collector).

**S8050 (NPN triode) in (a) & S8550 (PNP triode) in (b)**

![](./media/3bace56b6d4c5836d1f334038e88acf1.jpeg)

The S8050 transistor is a low-power NPN silicon tube and its the maximum voltage of collector and base can reach 40V and the current of the collector is (Ic) 0.5A.

The pins of the S8050 transistor should facing down, pin 1 is the emitter (E pole), pin 2 is the base (B pole), and pin 3 is the collector (C pole). Similarly, the S8550 transistor is the same.

![](./media/1337a16a23745afe86a78bbc628451f7.png)

![](./media/07ec79528ccc507de5c37057a48595a2.jpeg)

The commonly used triodes are divided into two types: PNP type triode and NPN type triode. S8550 is the PNP type triode, S8050 is the NPN type triode, what we provide in this kit are S8050 and S8550.

![](./media/5642275b2be86782bd9563ee840b0d1a.png)

#### 4. Connection Diagram 1：

We apply the S8050 (NPN triode) in this experiment to control the motor.

![](./media/5db0687f6510b28cf4ccee7aac0d7f93.png)

![](./media/319b4a31b0bc9d65d5f10bfcccf051a1.png)

#### 5. Test Code 1：

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny” , click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 17：Small Fan”. And double left-click the “Project\_17.1\_ Small\_Fan.py”.

![](./media/a5bc848c05c794a4b6b3f91d5310e27d.png)

```python
from machine import Pin
import time

motor = Pin(22, Pin.OUT)   # create S8050 object from Pin 22, Set Pin 22 to output

try:
    while True:
        motor.value(1)    # Set motor turn on
        time.sleep(4) # Sleep 4s
        motor.value(0)    # Set motoe turn off
        time.sleep(2) # Sleep 2s
except:
    pass
```

#### 6. Test Result 1：

Ensure that the Raspberry Pi Pico is connected to the computer, click“![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/5b4104877bd24416f5572a0a161aa6a3.png)

Click“![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts executing, we will see that The small fan turns for 4 seconds and stops for 2 seconds. Press “Ctrl+C” or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/d79dc606fd1e2ab55b51822fb5adb5e4.png)

#### 7. Wiring Diagram 2：

Control the motor with the S8550（PNP）triode

![](./media/3c3bfe5083b9b963b78e76c3b8d387db.png)

![](./media/08150e9b22904b62ff4b841a8551fbb6.png)

#### 8. Test Code 2：

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny” and click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 17: Small Fan”. And double-click “Project\_17.2\_ Small\_Fan.py”.

![](./media/af7e516a78e1cb0d6c5318954019f8ed.png)

```python
from machine import Pin
import time

motor = Pin(22, Pin.OUT)   # create S8550 object from Pin 22, Set Pin 22 to output

try:
    while True:
        motor.value(0)    # Set motor turn on
        time.sleep(4) # Sleep 4s
        motor.value(1)    # Set motoe turn off
        time.sleep(2) # Sleep 2s
except:
    pass
```

#### 9. Test Result 2：

Ensure that the Raspberry Pi Pico is connected to the computer，click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/acd099b78a9276a3f77ba78d53cfe732.png)

Click “![](./media/da852227207616ccd9aff28f19e02690.png)Run current script”, the code starts executing, we will see that The small fan turns for 5 seconds and stops for 2 seconds. Press “Ctrl+C” or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/3e2cb8a37e5525bfa433c3ca2e457d4a.png)

### Project 18: Dimming Light

#### 1. Introduction:

A potentiometer is a three-terminal resistor with a sliding or rotating contact that forms an adjustable voltage divider. It works by varying the position of a sliding contact across a uniform resistance. In a potentiometer, the entire input voltage is applied across the whole length of the resistor, and the output voltage is the voltage drop between the fixed and sliding contact.

In this project, we are going to learn how to use Raspberry Pi Pico to read the values of the potentiometer, and make a dimming lamp with LEDs.

#### 2. Components Required:

| ![b1265f71184b5d144248ea3e847a18c9](media/b1265f71184b5d144248ea3e847a18c9.jpeg) |![bbed91c0b45fcafc7e7163bfeabf68f9-16854050283871](media/bbed91c0b45fcafc7e7163bfeabf68f9-16854050283871.png)|![image-20230530081657284](media/image-20230530081657284.png)|![](media/ef77f5a64c382157fc2dea21ec373fef.png)|
| ------------------------------------------------------- | ------------------------------------ | ------------------------ | --------------------------- |
| Raspberry Pi Pico\*1                                    | Raspberry Pi Pico Expansion Board\*1 | Potentiometer\*1         | Red LED\*1                  |
| ![](media/wps73.png) |![image-20230529161414632](media/image-20230529161414632.png)|![c801a7baee258ff7f5f28ac6e9a7097b](media/c801a7baee258ff7f5f28ac6e9a7097b.png)|![](media/7dcbd02995be3c142b2f97df7f7c03ce-16854057420193.png)|
| Breadboard\*1                                           | 220ΩResistor\*1                      | Jumper Wires             | USB Cable\*1                |

#### 3. Component Knowledge:

![](./media/03ab81e8b4f09287d2781ef0fd297f85.png)

**Adjustable potentiometer:** 

It is a kind of resistor and an analog electronic component, which has two states of 0 and 1(high level and low level). The analog quantity is different, its data state presents a linear state such as 1 \~ 1024.

#### 4. Read the Potentiometer Value:

We connect the adjustable potentiometer to the analog IO of the Raspberry Pi Pico to read its value and voltage value . Please refer to the following wiring diagram for wiring.

![](./media/b8ee6320bce8729a4309857f257d30ec.png)

![](./media/cb970a340d830569e9ac4462a1318e44.png)

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 18：Dimming Light”. And double left-click the “Project\_18.1\_Read\_Potentiometer\_Analog\_Value.py”.

![](./media/b1fcd50c4db0ae1272b9b875f8003090.png)

```python
from machine import ADC, Pin
import time
# Initialize the potentiometer to pin 26 (ADC function)
adc = ADC(26)

# Print the current adc value of the potentiometer cyclically 
# Print the current voltage value of the potentiometer cyclically
try:
    while True:
        adcValue = adc.read_u16() # read the ADC value of potentiometer
        voltage = adcValue / 65535.0 * 3.3
        print("ADC Value:", adcValue, "Voltage:", voltage, "V")
        time.sleep(0.1)
except:
    pass
```


Ensure that the Raspberry Pi Pico is connected to the computer，click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend”.

![](./media/d7c9612533e1f601716f368cacca3586.png)

Click ![](./media/f79b2c42507d12b91ca23ea0bb87c5c2.png) “Run current script”, the code starts executing, we will see that the "Shell" window of Thonny IDE will print the ADC value and voltage value of the potentiometer, turn the potentiometer handle, the ADC value and voltage value will change. Press “Ctrl+C” or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/97f026e8fb8db1d28dd757e35c059d02.png)

![](./media/969b9de3cf505f05d6a9361286cef9c9.png)

#### 5. Circuit Diagram and Wiring Diagram:

In the last step, we read the value of the potentiometer, and now we need to convert the value of the potentiometer into the brightness of the LED to make a lamp that can adjust the brightness. The wiring diagram is as follows:

![](./media/66f721b77035d40556c873e0c4577b4a.png)

![](./media/93b03f3cdc8af506d9035b748839ac33.png)

#### 6. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny” , click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 18：Dimming Light”. And double left-click the “Project\_18.2\_Dimming\_Light.py”.

![](./media/308d874689ff5bf3cca0019a7b1bcf1f.png)

```python
from machine import ADC, Pin, PWM
import time

adc = ADC(26) # Initialize the potentiometer to pin 26 (ADC function)
pwm = PWM(Pin(16)) # Initialize the led's PWM to pin 16
pwm.freq(1000) # Define the PWM frequency as 1000
try:
    while True:
        adcValue = adc.read_u16() # read the ADC value of potentiometer
        pwm.duty_u16(adcValue) #map it to the duty cycle of PWM to control led brightness 
        time.sleep(0.1)
except:
    pwm.deinit()
```

#### 7. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”.

![](./media/6cf698bbc9ffac00f1e474eb554dde1d.png)

Click “Run current script”, the code starts executing, we will see that turn the potentiometer handle and the brightness of the LED will change accordingly. Press “Ctrl+C” or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/0bb12cb7c5842d8fbbd5d6d4684ad59e.png)

![](./media/eca30dead3f4923afa0dcb0306db2319.jpeg)


### Project 19：Flame Alarm

#### 1. Introduction:

Fire is a terrible thing and fire alarm systems are very useful in houses, commercial buildings and factories. In this project, we will use a Raspberry Pi Pico to control a flame sensor , a buzzer and LEDs to make fire alarm devices, which is a meaningful maker activity.

#### 2. Components Required:

| ![2e2bec86b3985dab2f1c07dfdb89ba73](media/2e2bec86b3985dab2f1c07dfdb89ba73.jpeg) | ![bbed91c0b45fcafc7e7163bfeabf68f9](media/bbed91c0b45fcafc7e7163bfeabf68f9.png) | ![image-20230530082616333](media/image-20230530082616333.png) | ![3ec5906fad2172708d449390140f55e6-168535106780428](media/3ec5906fad2172708d449390140f55e6-168535106780428.png) | ![4b4f653a76a82a3b413855493cc58fba](media/4b4f653a76a82a3b413855493cc58fba.png) |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| Raspberry Pi Pico*1                                          | Raspberry Pi Pico Expansion Board*1                          | Flame Sensor*1                                               | Red LED*1                                                    | Active Buzzer*1                                              |
| ![d5ce8dd2cc3fcf2acd49a27962911606](media/d5ce8dd2cc3fcf2acd49a27962911606.png) | ![3bdcc62cfa661d2b860a76e28537e21e](media/3bdcc62cfa661d2b860a76e28537e21e.png) | ![image-20230530082636422](media/image-20230530082636422.png) | ![image-20230530082656663](media/image-20230530082656663.png) | ![e9a8d050105397bb183512fb4ffdd2f6](media/e9a8d050105397bb183512fb4ffdd2f6.png) |
| Breadboard                                                   | USB Cable*1                                                  | 220ΩResistor*1                                               | 10KΩResistor*1                                               | Jumper Wires                                                 |

#### 3. Component Knowledge:

![](./media/a50ec3e38adf10643eafac8cb62bec8a.png)

**Flame Sensor**：

The flame emits a certain degree of IR light, which is invisible to the human eye, but our flame sensor can detect it and alert the microcontroller. If the Raspberry Pi Pico has detected a fire, it has a specially designed infrared receiver to detect the flame, and then convert the flame brightness into a fluctuating level signal. The short pin of the receiving triode is negative pole and the other long pin is positive pole. We should connect the short pin (negative pole) to 5V and the long pin (positive pole) to the analog pin, a resistor and GND. As shown in the figure below.

![](./media/87bd204db523c602c80745266c1ee452.png)

Note: Since vulnerable to radio frequency radiation and temperature changes, the flame sensor should be kept away from heat sources like radiators, heaters and air conditioners, as well as direct irradiation of sunlight, headlights and incandescent light.

#### 4. Read the Simulation Value:

We start with a simple code to read the value of the flame sensor and print it on the serial monitor. For wiring, please refer to the following wiring diagram.

![](./media/85531078db041bba05599b3a1118a7bc.png)

![](./media/1e3c424f7cc7ac797ab0b8ae4a00f4f1.png)

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → ”Project 19：Flame Alarm”. And double left-click the “Project\_19.1\_Read\_Analog\_Value\_Of\_Flame\_Sensor.py”.

![](./media/a2b329e2262514852ac484a2fda2a4a0.png)

```python
from machine import ADC, Pin
import time
# Initialize the flame sensor to pin 26 (ADC function)
adc = ADC(26)

# Read the current analog value of the flame sensor and return [0, 1023]
def get_value():
    return int(adc.read_u16() * 1024 / 65536)
 
# Print the current value of the flame sensor cyclically, value=[0, 1023]
while True:
    value = get_value()
    print(value)
    time.sleep(0.1)
```


Ensure that the Raspberry Pi Pico is connected to the computer, click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”.

![](./media/50455417516487c8495c097ad9f110db.png)

Click ![](./media/f79b2c42507d12b91ca23ea0bb87c5c2.png) “Run current script”, the code starts executing, we will see that the "Shell" window of Thonny IDE will print the simulation value read by the flame sensor. When the flame is close to the sensor, the simulation value increases. On the contrary, the simulated value decreases. Press “Ctrl+C” or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/370c5876c1ccf136fb1bd41335515c4d.png)

![](./media/7c04b9dd8c4a10e7b9788ecd95eeeeaa.png)

#### 5. Circuit Diagram and Wiring Diagram:

Next, we will use a flame sensor, a buzzer, and LEDs to make an interesting project, that is flame alarm. When flame is detected, the LED flashes and the buzzer alarms.

![](./media/c2b7feb8039e618ba070a9714ef06554.png)

![](./media/0cd1ee17a6f8de81464817090c5832eb.png)

#### 6. Text Code:

<span style="color: rgb(255, 76, 65);">Note：</span>![](./media/40a3ea572836945268b22dfc0cce29c3.png) The threshold of 500 in the code can be reset itself as required.

<br>
<br>

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 19：Flame Alarm”. And double left-click the “Project\_19.2\_Flame\_Alarm.py”.

![](./media/c863ab723600498531e50a6baa4bee19.png)

```python
from machine import ADC, Pin
import time

# Initialize the flame sensor to pin 26 (ADC function)
adc = ADC(26)
# create LED object from Pin 16,Set Pin 16 to output
led = Pin(16, Pin.OUT) 
# create buzzer object from Pin 17, Set Pin 17 to output
buzzer = Pin(17, Pin.OUT)   

# Read the current analog value of the flame sensor and return [0, 1023]
def get_value():
    return int(adc.read_u16() * 1024 / 65536)
 
# If the flame sensor detects a flame, the buzzer will beep and the LED will blink when the analog value is greater than 500. Otherwise, the buzzer does not sound and the LED goes off 
while True:
    value = get_value()
    if value >500:
        buzzer.value(1)    # Set buzzer turn on
        led.value(1)    # Set led turn on
        time.sleep(0.5) # Sleep 0.5s
        led.value(0)    # Set led turn off
        time.sleep(0.5) # Sleep 0.5s
    else:
        buzzer.value(0)    # Set buzzer turn off
        led.value(0)    # Set led turn off
```

#### 7. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”.

![](./media/a89a6364c773f77d114d4973ac957927.png)

Click ![](./media/f79b2c42507d12b91ca23ea0bb87c5c2.png) “Run current script”, the code starts executing, we will see that when the flame sensor detects the flame, the LED flashes and the buzzer alarms. Otherwise, the LED does not light, the buzzer does not sound. Press“Ctrl+C”or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend”to exit the program.

![](./media/ee561418efb12cc09b2a1448a7e2bda4.png)


### Project 20：Night Lamp

#### 1. Introduction:

Sensors or components are ubiquitous in our daily life. For example, some public street lights turn on automatically at night and turn off automatically during the day. Why? In fact, this make use of a photosensitive element that senses the intensity of external ambient light. When the outdoor brightness decreases at night, the street lights will automatically turn on. In the daytime, the street lights will automatically turn off. The principle of this is very simple. 

In this lesson we will use Raspberry Pi Pico to control LEDs to implement the function of this street light.

#### 2. Components Required:

| ![222aee34a428755aaf97b711ded3f09a](media/222aee34a428755aaf97b711ded3f09a.jpeg) | ![bbed91c0b45fcafc7e7163bfeabf68f9](media/bbed91c0b45fcafc7e7163bfeabf68f9.png) | ![d5ce8dd2cc3fcf2acd49a27962911606](media/d5ce8dd2cc3fcf2acd49a27962911606.png)     |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|                     Raspberry Pi Pico*1                      |             Raspberry Pi Pico Expansion Board*1              |                         Breadboard*1                         |
| ![image-20230530083727418](media/image-20230530083727418.png) | ![ef77f5a64c382157fc2dea21ec373fef](media/ef77f5a64c382157fc2dea21ec373fef-16854069210354.png) | ![df3db6765ee8c86beafa8410e87dd50d](media/df3db6765ee8c86beafa8410e87dd50d.png) |
|                       Photoresistor*1                        |                          Red LED*1                           |                         Jumper Wires                         |
| ![image-20230530082656663](media/image-20230530082656663.png) | ![image-20230530082636422](media/image-20230530082636422.png) | ![7dcbd02995be3c142b2f97df7f7c03ce](media/7dcbd02995be3c142b2f97df7f7c03ce-16854070557055.png) |
|                        10KΩResistor*1                        |                        220ΩResistor*1                        |                         USB Cable*1                          |

#### 3. Component Knowledge:

![](./media/9e553e75b6f976f33438171eb2f2e775.png)

It is a photosensitive resistor, its principle is that the photoresistor surface receives brightness (light) to reduce the resistance. The resistance value will change with the detected intensity of the ambient light . With this property, we can use photoresistors to detect light intensity.  Photoresistors and other electronic symbols are as follows:


![](./media/7d575da675a2f6cb511d28b801e2abaa.png)

The following circuit is used to detect changes in resistance values of photoresistors:

![](./media/5a7f7e641eb78007760a94151c1d80a5.png)

In the circuit above, when the resistance of the photoresistor changes due to the change of light intensity, the voltage between the photoresistor and resistance R2 will also change.  Thus, the intensity of light can be obtained by measuring this voltage.

#### 4. Read the Analog Value:

We first use a simple code to read the value of the photoresistor, print it in the serial monitor. For wiring, please refer to the following wiring diagram.

![](./media/e3fde13b200927346e04b032373ce638.png)

![](./media/b97ff27ae10e3499c36312c8ee4881f8.png)

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 20：Night Lamp”. And double left-click the “Project\_20.1\_Read\_Photosensitive\_Analog\_Value.py”.

![](./media/f4c9aec086f1f7661ea6b6d2cc39728d.png)

```python
from machine import ADC, Pin
import time
# Initialize the photoresistance to pin 26 (ADC function)
adc = ADC(26)

# Read the current analog value of the photoresistance and return [0, 1023]
def get_value():
    return int(adc.read_u16() * 1024 / 65536)
 
# Print the current value of the photoresistance cyclically, value=[0, 1023]
while True:
    value = get_value()
    print(value)
    time.sleep(0.1)
```


Ensure that the Raspberry Pi Pico is connected to the computer, click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)“Stop/Restart backend”.

![](./media/443211b5818f5f5af3a97f4c65866880.png)

Click ![](./media/f79b2c42507d12b91ca23ea0bb87c5c2.png) “Run current script”, the code starts executing, we will see that the "Shell" window of Thonny IDE will print the analog value read by the photoresistor. When the light intensity around the photoresistor is gradually reduced, the analog value will gradually increase. On the contrary, the analog value decreases gradually.

Press “Ctrl+C” or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/e018a1f56952b2a46f3e94d41a60e523.png)

![](./media/bbabb2d5c4a997c5024e6023cb272261.png)

#### 5. Circuit Diagram and Wiring Diagram:

We made a little dimmer in the front, now let's make a light controlled lamp. The principle is the same, the Raspberry Pi Pico will be used to obtain the analog value of the sensor and then adjust the brightness of the LED.  

![](./media/b8e8d95bdc869bf76465fa73645db831.png)

![](./media/71f2886dc6fa97d02e2ecd0d429af71b.png)

#### 6. Text Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → ”Project 20：Night Lamp”. And double left-click the “Project\_20.2\_Night\_Lamp.py”.

![](./media/bfd9c6083f4e9240de938f9241d9a039.png)

```python
from machine import Pin, ADC, PWM
import time

adc = ADC(26) # Initialize the potentiometer to pin 26 (ADC function)
pwm = PWM(Pin(16)) # Initialize the led's PWM to pin 16
pwm.freq(10000) # Define the PWM frequency as 1000
try:
    while True:
        adcValue = adc.read_u16() # read the ADC value of photoresistance
        pwm.duty_u16(adcValue) # map ADC value to the duty cycle of PWM to control led brightness
        time.sleep(0.1) # delay
except:
    pwm.deinit()
```

#### 7. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer，click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend”.

![](./media/830c67b94cb84c79b4f9df16fbfc07f2.png)

Click ![](./media/f79b2c42507d12b91ca23ea0bb87c5c2.png) “Run current script”, the code starts executing, we will see that when the intensity of light around the photoresistor is reduced, the LED will be bright, on the contrary the LED will be dim. Press “Ctrl+C” or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/c0e8ccda367bda88beef8852641040f6.png)



### Project 21：Temperature Instrument

#### 1. Introduction:

Thermistor is a kind of resistor whose resistance depends on temperature changes, which is widely used in gardening, home alarm system and other devices. Therefore, we can use this feature to make a temperature instrument.

#### 2. Components Required:

| ![2e2bec86b3985dab2f1c07dfdb89ba73](media/2e2bec86b3985dab2f1c07dfdb89ba73.jpeg) | ![bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556](media/bbed91c0b45fcafc7e7163bfeabf68f9-16853492486556.png) | ![b45bb81bb3763377c63accce606ac5f2](media/b45bb81bb3763377c63accce606ac5f2.png) |
| :----------------------------------------------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: |
|                     Raspberry Pi Pico*1                      |             Raspberry Pi Pico Expansion Board*1              |                         Thermistor*1                         |
| ![](media/wps73.png)| ![9232141f8a3166a8a6cdd43b78edd4e3](media/9232141f8a3166a8a6cdd43b78edd4e3.png) | ![image-20230529171550381](media/image-20230529171550381.png) |
|                         Breadboard*1                         |                       LCD 128X32 DOT*1                       |                        10KΩResistor*1                        |
| ![74ca4fa6d49dbd04de6a603c6e55a9ee](media/74ca4fa6d49dbd04de6a603c6e55a9ee.png) | ![df3db6765ee8c86beafa8410e87dd50d](media/df3db6765ee8c86beafa8410e87dd50d-16854075944518.png) | ![3bdcc62cfa661d2b860a76e28537e21e](media/3bdcc62cfa661d2b860a76e28537e21e.png) |
|                    10CM M-F Dupont Wires                     |                         Jumper Wires                         |                         USB Cable*1                          |

#### 3. Component Knowledge:

Thermistor: A thermistor is a temperature sensitive resistor. When it senses a change in temperature, the thermistor's resistance changes. We can use this feature to detect temperature intensity with thermistor. Thermistors and its electronic symbols are shown below:

![](./media/809b8634747fb295021f12e3b92b7894.png)

The relation between thermistor resistance and temperature is:

![img](media/wps1.png)

**Rt** is the resistance of the thermistor at T2 temperature.

**R** is the nominal resistance value of the thermistor at T1 room temperature.

**EXP\[n\]** is the nth power of e.

**B** is the temperature index

**T1** and **T2** refer to K degrees, that is, Kelvin temperature. Kelvin temperature =273.15 + Celsius temperature. For thermistor parameters, we use: B=3950, R=10KΩ, T1=25℃. 

The circuit connection method of thermistor is similar to that the photoresistor, as shown below :

![](./media/ac0d68aac58bffa5c99e1d0ed3a8bc37.jpeg)

We can use the value measured by the ADC converter to get the resistance value of the thermistor, and then use the formula to get the temperature value. Therefore, the temperature formula can be deduced as:

![img](./media/wps70.png)

#### 4. Read the Values:

First we will learn the thermistor to read the current ADC value, voltage value and temperature value and print them out . Please connect the wires according to the following wiring diagram.

![](./media/c143dc239ceaa5e65a63f47d6512630c.png)

![](./media/c0ad763fa1dda5ce55d03fe9b3d61bcd.png)

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny” , click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 21: Temperature Instrument”. And double left-click the “Project\_21.1\_Read\_the\_thermistor\_analog\_value.py”.![](./media/3377739fd44ab1dc80e11e1a99fb7abe.png)

```python
from machine import Pin, ADC
import time
import math

#Set ADC
adc=ADC(26)

try:
    while True:
        adcValue = adc.read_u16()
        voltage = adcValue / 65535.0 * 3.3
        Rt = 10 * voltage / (3.3-voltage)
        tempK = (1 / (1 / (273.15+25) + (math.log(Rt/4.7)) / 3950))
        tempC = int(tempK - 273.15)
        print("ADC value:", adcValue, "  Voltage: %0.2f"%voltage,
              "  Temperature: " + str(tempC) + "C")
        time.sleep(1)
except:
    pass
```


Ensure that the Raspberry Pi Pico is connected to the computer，click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/0181f74204e1aaa048e70d0a4f8b633d.png)

Click ![](./media/da852227207616ccd9aff28f19e02690.png)“Run current script”, the code starts executing, we will see that the "Shell" window of Thonny IDE will continuously display the thermistor's current ADC value, voltage value, and temperature value. Try pinching the thermistor with your index finger and thumb (don't touch the wire) for a while, and you will see the temperature increase. Press “Ctrl+C” or click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend” to exit the program.

![](./media/3ead8ea17c86c2cfbeffdb6b33985bad.png)

![](./media/0a035900fbc73a112eced64a926872ad.png)

#### 5. Circuit Diagram and Wiring Diagram:

<span style="color: rgb(255, 76, 65);">Note :</span> LCD\_128X32\_DOT must be connected with a 10CM M-F Dupont wire, the LCD\_128X32\_DOT will display normally. Otherwise, using a 20CM M-F Dupont wire may cause the LCD\_128X32\_DOT display abnormally.  

![](./media/281774a4fbf4f7f2ca0fd1e60c89516c.png)

![](./media/91445212232765942d482b84da03f598.png)

#### 6. Test Code:

The code used in this project is saved in the file **...\6.Codes\Python_Codes(Windows)**. We can move the code anywhere.  For example, we save the <span style="color: rgb(255, 76, 65);">Python_Codes(Windows)</span> in the Disk(D), <span style="color: rgb(0, 209, 0);">the route is D:\\Python_Codes(Windows)</span>.

Open “Thonny”, click “This computer” → “D:” → “Python_Codes(Windows)” → “Project 21：Temperature Instrument”. 

Select “lcd128\_32.py” and “lcd128\_32\_fonts.py”, right-click and select “**Upload to /**”, waiting for the “lcd128\_32.py” and “lcd128\_32\_fonts.py” to be uploaded to the Raspberry Pi Pico. And double-click the “Project\_21.2\_Temperature\_Instrument.py”.

![](./media/45d23c98bb87c3bfb1aee6093237ed9e.png)

![](./media/7b561df35f9e288c143ac6cc85ae9569.png)

![](./media/c9599c1346b7eaa605d6408a7013b16e.png)

```python
from machine import Pin, ADC, I2C
import time
import math
import lcd128_32_fonts
from lcd128_32 import lcd128_32

#Set ADC
adc=ADC(26)

#i2c config
clock_pin = 21
data_pin = 20
bus = 0
i2c_addr = 0x3f
use_i2c = True

def scan_for_devices():
    i2c = machine.I2C(bus,sda=machine.Pin(data_pin),scl=machine.Pin(clock_pin))
    devices = i2c.scan()
    if devices:
        for d in devices:
            print(hex(d))
    else:
        print('no i2c devices')

if use_i2c:
    scan_for_devices()
    lcd = lcd128_32(data_pin, clock_pin, bus, i2c_addr)

try:
    while True:
        adcValue = adc.read_u16()
        voltage = adcValue / 65535.0 * 3.3
        Rt = 10 * voltage / (3.3-voltage)
        tempK = (1 / (1 / (273.15+25) + (math.log(Rt/10)) / 3950))
        tempC = int(tempK - 273.15)
        
        lcd.Clear()
        lcd.Cursor(0, 0)
        lcd.Display("Temperature:")
        lcd.Cursor(1, 13)
        lcd.Display(str(tempC))
        lcd.Cursor(1, 16)
        lcd.Display("C")
        time.sleep(0.5)
except:
    pass
```

#### 7. Test Result:

Ensure that the Raspberry Pi Pico is connected to the computer, click “![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png)Stop/Restart backend”.

![](./media/5d60156d43ef268c27dfa9758bb53504.png)

Click ![](./media/f79b2c42507d12b91ca23ea0bb87c5c2.png)“Run current script”, the code starts executing, we will see that the LCD 128X32 DOT displays the voltage value of the thermistor and the temperature value in the current environment.

Press “Ctrl+C” or click ![](./media/27451c8a9c13e29d02bc0f5831cfaf1f.png) “Stop/Restart backend” to exit the program.

![](./media/5d60156d43ef268c27dfa9758bb53504.png)




