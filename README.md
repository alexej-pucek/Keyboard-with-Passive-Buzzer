**Keyboard With Passive Buzzer and Octave Changing**
In this project, I leveraged Buttons and Passive Buzzer that I have lying around, and build a working Keyboard. It is Piano Keyboard, but with the sound of Passive Buzzer, so buzzing. I used 13 Buttons for one octave 8 Full Tones, and 5 Semitones. I also Added 2 Buttons for changing the octave. There are 6 Octaves In total available (In the range of minimal and maximal frequency which can the Passive Buzzer produce. The lowest Tone is C2, and the highest is C8. I have used list of frequencies I have found online, but some of the frequencies had also decimal places, for example C2 = 65.41, which is a float value, and from what I know the buzzer can only output frequencies inputted as integers, so I had converted it to integers, as showed here: 

int C{65};
int D{73};
int E{82};
int F{87};
int G{98};
int A{110};
int H{123};
int C2{130};
int Cs{69};
int Ds{78};
int Fs{93};
int Gs{104};
int As{117};

(s means sharp, so for example Cs is C#)

To make multiple octaves, I learned that multiplying the frequency by 2 makes the tone 1 octave higher, so I programmed one button to multiply the frequencies by 2when pressed, and one to divide the frequencies by 2 when pressed. I also added a limiter, so when you reach octave 2, you can´t go lower, and if you reach octave 7, you can´t reach any higher, even if you keep pressing the buttons. 

Future plans:

1. Add display to show what tone is pressed, which octave are you currently on.
2. Replace the Passive Buzzer with Speaker, and add custom samples.


