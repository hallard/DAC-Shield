0-10V DAC / ADC / RS485 and OLED Arduino Shield
===============================================

This is a simple board to be able to 
- Generate 4 0-10V analog output to drive industrial devices
- 2 0-10V analog input (unprotected) 
- A RS485 Driver (use RX/TX of Arduino)
- 2 I2C Oled connector (Adafruit or Tindie Oled)
- 1 Rotary Encoder
- 1 WS2812B RGB Led

<strike>This is a proto board, I've just ordered one on OSHPark, will put 
more details once received and tested</strike> This shield has been fully tested and it's working fine. The only problem was my bad datasheet reading, the DAC7565 output from the chip are not 0V 5V as I expected but 0V 2.5V (internal VREF) So as I multiply ouput per 2, the output for these 4 outputs are 0V-5V not 0V-10V, you can change the multiplier by changing resitor R2/R4/R6/R8 from 10K to 30K.

I wrote an Arduino Library to drive the DAC7565 [here][3]

Check out news and other projects on my [blog][4]

Detailed Description
====================

Everything will be documented on my [blog][4]

**Schematic**  
![schematic](https://raw.github.com/hallard/DAC-Shield/master/dac-shield-sch.png)

**Board**  
![board]( https://raw.github.com/hallard/DAC-Shield/master/dac-shield-brd.png )

![top](https://raw.github.com/hallard/DAC-Shield/master/dac-shield-top.png)&nbsp;&nbsp;![bottom](https://raw.github.com/hallard/DAC-Shield/master/dac-shield-bottom.png)

[3]: https://github.com/hallard/DAC7565
[4]: http://hallard.me


