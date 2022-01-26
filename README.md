# hc-sr501
PIR sensor

If you didn’t know, all objects with a temperature above Absolute Zero (0 Kelvin / -273.15 °C) emit heat energy in the form of infrared radiation, including human bodies. The hotter an object is, the more radiation it emits.

PIR sensor is specially designed to detect such levels of infrared radiation. It basically consists of two main parts: A Pyroelectric Sensor and A special lens called Fresnel lens which focuses the infrared signals onto the pyroelectric sensor.

A Pyroelectric Sensor actually has two rectangular slots in it made of a material that allows the infrared radiation to pass. Behind these, are two separate infrared sensor electrodes, one responsible for producing a positive output and the other a negative output. The reason for that is that we are looking for a change in IR levels and not ambient IR levels. The two electrodes are wired up so that they cancel each other out. If one half sees more or less IR radiation than the other, the output will swing high or low.

When the sensor is idle, i.e. there is no movement around the sensor; both slots detect the same amount of infrared radiation, resulting in a zero output signal.

But when a warm body like a human or animal passes by; it first intercepts one half of the PIR sensor, which causes a positive differential change between the two halves. When the warm body leaves the sensing area, the reverse happens, whereby the sensor generates a negative differential change. The corresponding pulse of signals results in the sensor setting its output pin high.

The basic Info about the sensor is give below

![Screenshot 2022-01-26 212020](https://user-images.githubusercontent.com/96690206/151197472-f2890a50-db63-4015-9076-e09350bdb83e.png)
HC-SR501 PIR sensor has three output pins VCC, Output and Ground as shown in the diagram below. It has a built-in voltage regulator so it can be powered by any DC voltage from 4.5 to 12 volts, typically 5V is used.

VCC is the power supply for HC-SR501 PIR sensor which we connect the 5V pin on the Arduino.

Output pin is a 3.3V TTL logic output. LOW indicates no motion is detected, HIGH means some motion has been detected.

GND should be connected to the ground of Arduino.
![Screenshot 2022-01-26 212224](https://user-images.githubusercontent.com/96690206/151197783-75decfc1-f930-4850-b87e-f08ff063098e.png)



This is the interfacing PIR with Arduino.

![pir](https://user-images.githubusercontent.com/96690206/151197080-a581f566-6597-4fbe-b0af-678029f0834f.png)
