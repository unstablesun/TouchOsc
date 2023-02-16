Midi Note Pad.  This is my first project after a day looking through the docs and the excellent community posts on the TouchOsc Discord.

This is a very basic/beginner example of creating a grid of buttons and lables and sending midi information out based on the note pressed.
I also tried to make this quick and simple and did not "ungroup" the grid which was my first impluse, ha ha.




![image](https://user-images.githubusercontent.com/8905472/219409314-85da6912-e036-4400-ae01-5c222a4ef196.png)


First create a group, double click on the group to get inside and create two grids.

![image](https://user-images.githubusercontent.com/8905472/219444546-8efdd3a1-4549-4932-b35e-b803dcae2fae.png)

The first grid is of type BUTTON.  Set the rows and columns and anything else you want.  Note any change you make to the button grid must match the lable grid as far as dimensions and orientation.

![image](https://user-images.githubusercontent.com/8905472/219445922-a487111c-f32b-4216-91d3-5e97087f2b67.png)



Do the same for the label grid but make it of type LABEL.  Also uncheck the following.

![image](https://user-images.githubusercontent.com/8905472/219447929-f2a412b1-fbd7-40c7-8cf6-3fc48ad9ff8e.png)

Ok this is the key part, back to the button grid and to the midi message. Change to NOTE_ON.  For the Note INDEX set the scale to your root note and the other value to root note + 1?  I'm not really sure why this works. I fiddled with these values till I got it working but the end result is that all the buttons in the grid will have a sequencial sequence of midi notes 60 - 72.



![image](https://user-images.githubusercontent.com/8905472/219448670-d0dc7385-0e63-43d2-a2d5-36e194127f2f.png)

