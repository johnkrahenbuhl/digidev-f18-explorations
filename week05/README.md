<h1>Week 05: Arduino LCD & IR - Bonus Raspberry Pi 7' LCD with Capacitive Touch Screen
<h4>Fall 2018 IIT Institute of Design Introductory Course to Arduino/Raspberry Pi and Development for Wearable Devices

<h6>Explorations and Coursework by John Krahenbuhl </br></br></h2>

<h2>ARDUINO</h2> 
</br>

<h2>RASPBERRY PI 3 B</h2>


[LANDZO 7 INCH LCD SCREEN: HDMI WITH USB CAPACITIVE TOUCH](https://www.amazon.com/LANDZO-Touch-Screen-Raspberry-Display/dp/B01ID5BQTC/ref=sr_1_1?ie=UTF8&qid=1537481301&sr=8-1&keywords=landzo+7+inch+screen)
</br>
![Landzo 7 In LCD Screen](https://images-na.ssl-images-amazon.com/images/I/41ExtMMYuUL._AC_US436_FMwebp_QL65_.jpg)
</br>
To enable the screen connect the HDMI and USB cables between the screen and Pi. From [comments on Amazon](https://www.amazon.com/gp/customer-reviews/R26HDWFDBTFYXY/ref=cm_cr_srp_d_rvw_ttl?ie=UTF8&ASIN=B01ID5BQTC) add the following to the bottom of your `/boot/config.txt` file:</br>
```
max_usb_current=1
hdmi_group=2
hdmi_mode=1
hdmi_mode=87
hdmi_cvt 800 480 60 6 0 0 0
#Resolves pink line with on the left for rpi3 with Jessie.
hdmi_drive=1
```

Then reboot your Pi:  
```

sudo reboot

```

When the Pi reboots, your screen should be working.</br></br></br>

**ADDING A TOUCHSCREEN KEYBOARD**</br></br>
![Matchbox Keyboard](https://mcuoneclipse.files.wordpress.com/2015/12/virtual-keyboard.png)</br></br>
I installed the *Matchbox Keyboard* using the following:</br>
[ModMyPi Matchbox Keyboard Tutorial](https://www.modmypi.com/blog/matchbox-keyboard-raspberry-pi-touchscreen-keyboard)</br>

</br>After installing the *Matchbox Keyboard* I added a button to the *Launchbar* following:</br>
[RaspberryPi.org Blog Post](https://www.raspberrypi.org/forums/viewtopic.php?t=112515)

</br></br>*Note: Thanks to @zachpino for mentioning Git Markdown!*
