# DIGITAL-STOP-WATCH-USING-555-TIMER-IC
IC Applications
A stopwatch is a timer that is used to measure an event anywhere from milliseconds to several hours. We can start and stop the count of the stopwatch at any instant and it can also be reset to zero to measure the timing of a new event.
Stopwatches need no introduction; we use them at many points in our lives to measure timings for several purposes, like during cooking to avoid the food being overcooked or undercooked, during a sports event, or even at the science lab.
Stopwatches may be analog or digital. Digital stopwatches are much more common than analog versions, owing to their higher accuracy and ease of use. Here we have tried to realize a digital stopwatch of reasonable accuracy and reliability. 
The stopwatch we are going to design is accurate up to one-tenth of a second. The circuit is relatively simple and easy to realize. An astable multivibrator serves as the circuit's primary component, along with the counter and decoder stages.
The 555 timer IC is an 8-pin integrated circuit used in a variety of timer, pulse generation, and oscillator applications. The 555 can be used to provide time delays or as an oscillator.
We also use IC 4026, which is counter and seven-segment decoding in one package IC, which is very easy to interface with seven-segment displays. This is a fully static counter-operational IC and is ideal for low-power displays. 
This IC can be used for decade-counting seven-segment decimal displays, frequency division seven-segment decimal displays, clocks, watches, timers, and counter/display drivers for meter applications. 
The circuit operates on a 5-volt DC supply. It uses a seven-segment LED display of common anode type to show time.


CIRCUIT DIAGRAM:                                                        // In PROTEUS

![image](https://github.com/ChinmaiChowdary/DIGITAL-STOP-WATCH-USING-555-TIMER-IC/assets/119433702/b38120e2-9ab1-412e-a0b7-09afa320ea6e)



In this circuit, we have used a 555 timer IC-based a-stable multivibrator, which is for creating a 1-second delay. And two common cathode seven-segment decoder ICs, namely CD4026. The output of the A-stable multivibrator is directly applied to the seven-segment decoder's (U2) Clock pin (1) and carry output pin (5) of the U2 IC is directly connected to the clock pin (1) of the second seven-segment decoder (U1). And seven segments are connected with this decoder (U1 and U2). Its connections are shown in the stopwatch circuit diagram given below. One push button is used to stop or start the stopwatch and one push button is used to reset the stopwatch. A 5-volt voltage regulator is used to provide 5 volts to the whole circuit. A 9-volt battery is used for powering the circuit. The rest of the connections are shown in the circuit diagram.

Working:

In this stopwatch circuit, we have generated a second delay by using a 555 timer based on a stable multivibrator. By using some calculation we can easily generate a second delay. In a stable multivibrator, there are two resistors, and one capacitor is responsible for delay by charging or discharging a capacitor through resistors. The calculation formula for generating delay for a stable multivibrator is given below. F=1/T= 1.44/(R1 + 2R2) C1.
In this project, we have selected R1 as 60K, R2 as 30K, and C1 as 10uF. As an A-stable multi-vibrator generates a one-second delay, this delay is oscillations or pulse of 0 and 1. So we will use this pulse to trigger the seven-segment decoder, and then the segment decoder will change the digit number within the one-second time period. When we ON the stopwatch (by start/stop button), it starts counting from zero and if we turn OFF the same button again or press the reset button. There are two segments, so this stopwatch circuit can count from 00 to 99 seconds.


OUTPUT:

![image](https://github.com/ChinmaiChowdary/DIGITAL-STOP-WATCH-USING-555-TIMER-IC/assets/119433702/e69d451a-3820-4716-9deb-bcc2eaf74e80)


Simulation Output:

![image](https://github.com/ChinmaiChowdary/DIGITAL-STOP-WATCH-USING-555-TIMER-IC/assets/119433702/0a56c3fe-69ac-4871-854c-7f808391b410)
