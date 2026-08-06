# Smartwatch Interface
This is my first hardware related project, in which I use a [*Grove Beginner Kit for Arduino*](https://www.seeedstudio.com/Grove-Beginner-Kit-for-Arduino-p-4549.html) (the only thing in my BOM) to create a interface on the OLED Display which is supposed to somewhat imitate a smartwatch.

Although it makes use of an OLED Display, Piezo Buzzer, Button, Rotary Potentiometer, Sound Sensor and a Temperature & Humidity Sensor, I would consider this to be mainly a software project as the whole time I spent on this (roughly 11 hours), was writing the code.

It was very satisfying to write as I had to solve problems like how to get multiple inputs with only a button and a potentiometer, and I ended up using short and long button presses for different input types.

Its features are:
- A password input screen, in which you need to input a 4 digit code, and can only see the main screen if logged in
- A lockdown script, so if you enter an incorrect password more than 2 times it locks you out for a certain amount of times (depending on number of consecutive incorrect login attempts)
- A clock (although it does not know the actual time and assumes time of boot is 12pm)
- A stopwatch with abilities to stop, start from the stopped time, and reset
- A timer for 1 min, 5 min and 10 min, with abilities to pause and restart the timer
- Temperature + Humidity display 
- Sound Monitor, which tells you to stop yelling if the sound quantity is above the sound limit
- Settings, in which you can edit the time format (am+pm/24 hour), sound limit (300/500/700), and temperature unit (C/F)


I learnt a lot about writing code for hardware, how to refactor code so it uses as less memory as possible, how to only redraw the screen when new content is registered, and how to get sensor data as input.

This is how the start looked:
<img width="666" height="347" alt="Screenshot 2026-08-06 at 17 38 37" src="https://github.com/user-attachments/assets/88967082-1c3f-4462-b0f8-7a3963b6f02e" />
And the full demo is on the Macondo project page: https://macondo.hackclub.com/projects/13737
