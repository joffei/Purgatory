# Purgatory
Terribly hard maze game based off of the Basic Stamp 2 (BS2)

<----------GAME PLAY----------><br>
* Hook up power and tilt the BS2 board in the direction in which you want the ball to roll.
* The ball may roll left, right, up, down, or diagonal in any direction.
* Avoid the obstacles (black boxes), a single touch will lose the game
* ******BE AWARE OF THE INVISIBLE MIDDLE LINE******
* You must go to the end of the top half of the screen to get to the bottom half of the screen
* Get to the finish line (the  open box) in as little time as possible in each level
* Once a level is finished, the next will immediately start in the same orientation, with the finish line changed
* To pause, push the button during game play
* To Unpause, push the button while game is paused, and be set back where you left off
* Once the user loses and the game ends, a message will display the level the user ended on and the time taken to get to the level (not the time ended)

<---------LEADERBOARD---------><br>
* If you can get to  ranking level in the least amount of time, you will qualify for the leaderboard.
* An entry will appear after 3 seconds with 3 spaces for character input.
* Push the button to change the character in the input field.
* Valid input characters are all uppercase English Letters as well as "[", "\", "]", "^", "_", and " ".
* When the correct letter has been selected, wait 2 seconds to go advance to the next character
* *******THERE IS NO WAY TO GO BACK*******
* Once all the characters have been selected, the screen will wipe clean and the name will be added to leaderboard
* To view the leaderboard, press and hold the button outside of gameplay.

<-----REQUIRED MATERIALS------><br>

| Quantity      |Item                                   |<br>
| :-----------: | :-----------------------------------: |<br>
| 1             |Basic Stamp 2 (BS2) Homework Board     |<br>
| 1             |9V DC Battery                          |<br>
| 7             |Jumper Wires                           |<br>
| 1             |Memsic Dual-Axis Accelerometer         |<br>
| 1             |4-Pin Push Button                      |<br>
| 4             |220K Ohm Resistors                     |<br>
| 1             |Serial LCD Display Model# 27979        |<br>
| 3             |Male/Female Extension Wires (Optional) |<br>


<------------SETUP------------>
1. Place the accelerometer in the middle of the board accross the center divider
2. Use 2 resistors to hook the left middle pin of the accelerometer to pin 7 and the right middle pin to pin 6
3. Use a jumper wire to connect the left bottom pin of the accelerometer to Vss (GND)
4. Use a jumper wire to connect the right top pin of the accelerometer to Vdd (+5V)
*Follow the diagram below <br>
                  ___<br>
                -|   |---->+5V<br>
        P7<--^^--|   |--^^-->P6<br>
         GND<----|___|-<br>

^^ = resistor<br>

5. Place the push button at the bottom of the board accross the center divider
6. Use a resistor to connect the bottom left pin of the push button to pin 0
7. USe a resistor to connect the bottom right pin to Vss (GND) (You may want to use a jumper wire for extra length)
8. Use a jumper wire to connect the left top pin to Vdd (+5V)
* follow the diagram below<br>
                  ___<br>
         +5V<----|   |-<br>
        P0<--^^--|___|--^^-->GND<br>

^^ = resistor<br>

9. Use 3 jumper wires to connect the LCD to Pin 14, Vdd (+5V), and Vss (GND) from top pin to bottom pin
	*You may find it easier to use the 3 extension wires in the case
	NOTE: make sure that the pin 14 is not connected without Vdd (+5V) also connected
*Follow the diagram below<br>
                            ______________________________________<br>
                   P14<----|                                      |<br>
                   +5V<----|                 LCD                  |<br>
                   GND<----|                                      |<br>
                           |______________________________________|<br>