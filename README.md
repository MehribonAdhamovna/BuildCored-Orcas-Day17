# BuildCored-Orcas-Day17
PWMSimulator  — BUILDCORED ORCAS Day 17

What it does. This simulator uses a slider to change how fast a digital signal switches between "on" and "off," which makes a virtual LED look like it's smoothly changing brightness. It visually shows that a higher "on-time" (duty cycle) results in a higher average voltage.

Hardware concept. Pulse Width Modulation (PWM) is a trick microcontrollers use to fake an analog voltage (like 1.65V) using a digital pin that can only do 0V or 3.3V. By blinking the pin faster than the eye can see, the hardware creates an "average" power level that controls things like LED brightness or motor speed.

What I would do differently. I’d add a second slider and a second wave line to the graph with a different frequency (like 500Hz) to show that multiple PWM channels can run independently. I would also explain that the average voltage is simply the Supply Voltage × Duty Cycle percentage, which is why 50% duty gives exactly half the max brightness.

Run it. python day17_starter.py
