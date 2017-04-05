# WasteSort
Hack Davis Project

What it does
It is a system which guides people into maintaining a cleaner environment by scanning trash and classifying it as compost, recycle, or landfill.

How we built it
We created a tensor flow environment on raspberry pi which displayed the outputs of the neural network as a character. The program starts when the button is pressed on the breadboard which takes a picture and scans it and classifies the image as compost, recycle, or landfill against the neural network. According to the classification, the result is outputted as a text file and then displayed on the corresponding LED on a breadboard.

#Files
Switch.py - Interfaces with Raspberry Pi 3 GPIO pins to trigger inputs and outputs to the embedded system (LEDS and Sensors in this case)
label_image.py - Runs the retrained version of Google's Inception to detect objects.
