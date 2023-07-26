About me

My name is Mi-ann Wirjosentono. I am from Santo Boma,Wanica and. I am currently 17 years old and I will be starting my second year of VWO. 

![](https://lh6.googleusercontent.com/2m5Q06DGRE12UhwExjq4TvrGDimpMUROxrafxoJTS61HlNV28lKBrLA61COb21mAg-S9CqwWSgJeg6-LMkUNh50LLkV5j0ecQgCzbinl_s6hiHQbdA8AJJxDr_35ptRMge0t5t3ANyZ3yflJj0fpqBk)

I applied for the program because I want to develop my skills and learn about coding and building things. My dad also liked to develop circuits in his spare time. I have always liked to learn things in my spare time and I like physics as well as reading and writing. I also like to things that are difficult to solve.

Day 1 September 5th 2022

Objective:

introduction:

Introduction to the 3 types of circuits and its components

Introduction to Arduino

Build a basic blinking led

Component list:

AAA 1.5 V battery

9V battery 

resistors 

diode

led 

breadboard

multimeter

Arduino uno

Pushbutton

Circuits

First there was a quick review on what electricity was and referred to as water on a mountain.

Electricity consists of current, potential energy and resistance.

the law potential energy is equal to the current times the resistance.

 We were introduced to the follwing 3 types of circuits:

1.  Simple circuit

2.  serie circuit

3.  parallel circuit

4.  arduino circuit

1.  Simple circuit

Here I learned how to select three AAA 1.5V batteries on tinkercad and to couple it to a led. A resistor must be placed between the anode and positive pole of the battery to prevent it from blowing up.

1.  Serie circuit

Here I used a 9V battery and 3 led lights. I coupled the leds together by connecting the anode of one led to the cathode of the other. I then coupled the free anode to the positive pole via a resistor and the free cathode to the negative pole of the battery.

3  parallel circuit

Here I once again used a 9V battery and 3 lights. However I coupled a diode with the positie pole to let the current flow in only one direction. From the diode I placed 3 separate cables each going to a cathode of a led. Then I placed another diode and coupled 3 seperate cables to for the cathode of each led. This diode I then coupled to the negative pole of the battery

Then I used a breadboard and a multimeter to check the resistance of the resistors. I was taught how to check the resistance of resistors of both parallel and serie circuit situations

4\. Arduino Circuit

I used an arduino uno R3 and a breadboard. This I coupled with a potential energy of 5v from the power section to the bottom of the breadboard with the plus sign.and groundpin to the bottom of the breadboard where the minus sign is. In the row where the groundpin is connected I placed a resistor and placed a led in the upper row of the 3rd section of the breadboard with the cathode being in the same column as the resistor. From the Digital section I coupled number two with the bread board one row above the resistor in the column where the led's anode is.

![](https://lh3.googleusercontent.com/xnSmc8mZ763ZPHvmaBJF2CsDEToZ_TOsrI75a-2VWXQkoS66_sr_oIW0kg9WyYYWVf_GZV1aNqSMmY7M7KfyD9Q8vdyW6WwSLowWyHhaHWIc8cMU8ZVNxkYF-m8rfqzgSfyozVzma8a2Dwh9u1wUW2M)

Then I added a pushbutton. Terminal 1a and 2a were in same row as the led light but 7 coloms away from it  To connect this I connected the positive cable of bottom section to the top section's plus sign row aswell with the negative cable to the top section's minus sign row. In the row of the latter I placed a resistor horizontally in the same colomn as terminal 2b  and parallel to it as well as evenly long I placed a cable in the colomn of terminal 1b.

Then I typed the code to make the light turn on and flicker.

Code

int led = 2;

int button= 3;

void setup () {

pinMode (led,  OUTPUT);

pinMode(button.  INPUT);

}

void loop () {

if (digitalRead(button)== High)

{

digitalWrite (led, HIGH);

delay (500) 

digitalWrite (led, LOW);

delay (500)

}

else 

{digitalWrite (led,  HIGH);

}

}

mistakes:

I coupled the cables wrong a couple times during the arduino circuit because i didnt fully understand what I was doing. During coding I also made some mistakes Sometimes I accidentally deleted the entire lines of code and sometimes I forgot the curly brackets or ";" sometimes I pressed "shift+:" sometimes I forgot how to continue editing a design after accidentally leaving.

note to self: edit = press tinker

DAY 2: SEPTEMBER 6TH 2022

Objective:

Introduction to analog In 

Built a circuit with a potentiometer

Built a circuit with a temperature sensor

Components:

Arduino Uno

Breadboard

Led

potentiometer

temperature sensor

resistors

Lesson:

-quick review/ mention of yesterdays leerstof 

-analog vs digital: digital can only turn led on and off, analog lets you turn on and off and in between, lets you dim the led and switch between leds 

- we learned about conditions

dimmer circuit (potentiometer)

-place an arduino uno and a breadboard next to each other. connect power (5v) to power sign on the breadboard (bottom section) and ground to the ground sign on the breadboard ( also bottom section)

![](https://lh5.googleusercontent.com/_0CcchL0nAK3nhS9gvmMXYGYnkElluxzXoO81BXQ-IQTCUbDnn_RehXxj2PKfhG1XQT_wKx7JRtGE2PwDu7BqVMBJcNcUWbp9iqNArpKEo9ijoRwtZRwnf8RSOm6escFEVtCpzVS9Q4t_LAF49L3jvA)

-place potentiometer on row d and connect terminal 1(pot) to ground, wiper to A0 and terminal 2 to power 

-place led on row e, connect cathode to ground place resistor on row d for led anode and connect to digital pin 3

after typing the code serial mode should go from 0 to 1023 when turning the potentiometer knob from left or right

-   Led should turn darker when turned left and brighter when turned  right

code:

int pot=A0;

int Led = 3'\;

void setup ()

{

Serial.begin (9600);

pinMode (Led, OUTPUT)

}

void loop ()

{

int pot_value = analogRead(pot)

Serial.println (pot_value);

int Led_value = map (pot_value, 0, 1023, 0, 225)

digitalWrite(Led,  Led_value)

}

mistakes

-My mistakes were made during coding. It takes me a while to write which makes me lose track of where we are in the lesson. I also wrote part of the code wrong which gave me a ot of errors

-at the end of int sentence always put ;

Dimmer circuit (temperature sensor)

-place arduino board uno and breadboard. 

- Connect power (arduino, 5V) with powerline (breadboard) 

 Ground (arduino) with groundline(breadboard)

![](https://lh6.googleusercontent.com/HZD9YC9u2IDV5eD2VQkbm3U89Bpwb7yeRDo7q3NYxP7A12GRf6bX49rMz3s011Jr5yBrdftlEvqBmcHLtaBspU4ujrEha1JYoz4FqbgQQR-IX5mBmFJRjmps7BPKaMFBDzjnAPmr0sIqvC7xV2EKfVk)

-Place Temperature sensor (row: e. column: 10)

connect powerline(breadboard) to power(temperature sensor), 

groundline (breadboard) with ground (temperature sensor) 

vout with A0

- place Led2 (blue) (row: g; column: 16 (cathode), 17 (anode))

connect cathode to ground line

connect resistor to anode 

connect pin 2 to anode & resistor ((row: a, column: 17)

-place Led1(blue) (row: g; column: 18 (cathode), 19 (anode))

connect cathode to ground line

connect resistor to anode 

connect pin 3 to anode & resistor ((row: a, column: 19)

in simulation: 

when the temperature sensor's value greater than 100 Led1 1 will turn on

when the temperature sensor sensors the  temperature is equal or less than 100Led2 will turn on

code:

int temp = A0;

int Led1 = 3;

int Led2 = 2;

void setup ()

{

serial.begin (9600);

pinMode(Led1,  OUTPUT);

pinMode (Led2.  OUTPUT);

}

void loop ()

{

int temp_value = analogRead(temp);

Serial.println (temp_value);

int Led_value = map (temp_value, 20, 358, 0, 255);

if (temp_value > 100)

{

digitalWrite(Led1, HIGH);

digitalWrite(Led2, LOW);

}

else 

{

digitalWrite(Led1, LOW);

digitalWrite(Led2,  HIGH);

}\
}

Mistakes

I made mistakes during coding here as well. Sometimes I forgot to declare. Sometimes I put the wrong bracket or put this sign ";" too much.  sometimes I put a dot instead of a comma. Sometimes I couldnt keep up but I started getting the hang of things.

DAY 3 SEPTEMBER 7TH 2022 

Objective:

-   introduction Pwm

-   Introduction micro servo & DC motor

-   control micro servo with PWM

-   control DC motor with PWM

components: : 

-   arduino uno 

-   breadboard

-   micro servo

-   potentiometer

-   9v battery

-   power supply

-   dc motor

-   L293D

Lesson: 

-   quick review on the previous lesson

PWM vs regular Digital pins

digital pins only let  one turn a led off or on . Through PWM One can control the voltage to change and manipulate the current to slowly turn on or turn off. This is needed to control the speed at which an object will move. important when programming robots in the future. We let de object move in degrees like doors spinners motor

micro servo circuit

-place arduino uno and breadboard

connect power (arduino, 5V) to powerline (breadboard, bottom section)

connect ground (arduino) to groundline (breadboard, bottom section)

![](https://lh4.googleusercontent.com/w-E1598eaJ2il0X7YIyjtqs-kfz8qmcM9E1dn4Lu5pU_Dk6OiigTlq9rwsyfcQxHTreglmeXd2BmInf5l601VZ25-8xM0WLnSJCU3G-ZKd3z34Uxm9lt0UCZE7jzF40fS71jb1aaDLsTZO5-7sxZYDE)

-place  micro servo 1 (star, bottom)

connect ground (micro servo) to ground line (Breadboard, bottom section)

connect power (micro servo) to power line (breadboard, bottom section)

*connect signal to  PWM 3

-   then write code to let the spinner spin to o degrees then 90 then 180 and back to 0

-   also let serial print be seen

-   after code connect bottom section's  ground line to top section's groundline 

-   place  micro servo 2 (Ana, top micro servo)

-   connect ground (micro servo) to ground line (Breadboard, top section)

-   connect power (micro servo) to power line (breadboard, top section)

-   *connect signal to  PWM 5

-   let it spin the same as the first

first code;

#include  <Servo.h>

Servo star;

int servoPin = 3;

void setup()

{

star.attach(servoPin);

Serial.begin (9600);

}

void loop ()

{

star.write(0);

Serial.println ("0 degrees");

delay(2000);

star.write(90);

Serial.println ("90 degrees");

delay(2000);

star.write(180);

Serial.println ("180 degrees");

delay(2000);

}

second code:

#include  <Servo.h>

Servo star;

Servo Ana;

int servoPinstar = 3;

int seroPinAna = 5;

void setup()

{

star.attach (servoPinstar);

Ana.attach (servoPinAna);

Serial.begin (9600);

}

void loop ()

{

star.write(0);

Ana.write(0);

Serial.println ("0 degrees");

delay(2000);

star.write(90);

Ana.write(90);

Serial.println ("90 degrees");

delay(2000);

star.write(180);

Ana.write(180);

Serial.println ("180 degrees");

delay(2000);

}

mistakes

no mistakes until the 2nd code. I wasnt sure what to code to make the second micro servo spin like the first. I failed 2-3 times. after namimng my second servo I wasnt sure how to continue I tried renaming int servoPin = 3 to servoPin(star) but it wanted to be read as Servo. 

I tried to write

int servoPin = 3

int servoPin = 5 

but it didnt work

after looking at the code and retryingI ended up changing "int servoPin = 3' to "int servoPintar =3 and the next code of line to int servoPinAna = 5

as well as  adding 

Ana.write(0)

Ana write(90)

Ana.write(180)

to the lines within brackets for void loop)  as seen above  "second code)

Control micro servo with potentiometer

--place arduino uno and breadboard

connect power (arduino, 5V) to powerline (breadboard, bottom section)

connect ground (arduino) to groundline (breadboard, bottom section)

![](https://lh5.googleusercontent.com/siTEzrp7BXSAdIH9-ePSwjOwVdn3v7z-h8E29yJOwTRftqblQ8isoZ9a5WtewStd75W4t9oqBC5mUC5Ny6xgu-8newxTBeq2_5HVvwSFBNyMOnxMGaCujmWcTbkBFdxlkJF8hWXLqxci6dCGOZVqXZs)

-place  micro servo (star, bottom)

connect ground (micro servo) to ground line (Breadboard, bottom section)

connect power (micro servo) to power line (breadboard, bottom section)

*connect signal to  PWM 3

--place potentiometer on row d and connect terminal 1(pot) to ground(arduino), wiper to A0 and terminal 2 to power (arduino)

-type in code

-after writing one should be able to control the spinning of the micro servo through the potentio meter

Code 

#include  <Servo.h>

Servo star;

int servoPin = 3;

int pot = A0;

int potValue;

int ServoValue;

void setup ()

{

star.attach (servoPin);

serial.begin(9600);

}

void loop ()

{

potValue = analogRead(pot)

ServoValue = map (potValue, 0, 1023, 0, 180)

star.write(ServoValue)

Serial.println(ServoValue)

}

mistakes 

Sometimes I forgot to declare although it is less now. Sometimes i put small letter in stead of capital. Sometimes i put capital letter instead of small letters.

DC motor  control

DC motor and 9V battery

*changing polarity= changing the direction the motor spins

-   if red is connected to red and black to black it will spin forward(rmp: positive)

-   if red is connected to black and black to red it will spin backward(rmp:negative)

![](https://lh4.googleusercontent.com/hoDZiYa_kZowblYG26sBXb0X9_I95R0xIb8zOxkVZYa3ALeK2O70Fto7NoyCB8WyBmKBm1d4gITev2Ykov68aBvFkvrOtCIZOZS96dd0NyK2327pEC2PdJiG9hEn7wLi3vhNNbAmy3TcJV7WTakBoFU)

mistakes; none

code: none

DC motor & Power Supply

-increase/decrease in voltage = increase/ decrease in speed

-turning the knobs of the power supply let you control de speed of the motor

   lower is slower higher is faster

mistakes: none

code: none

![](https://lh5.googleusercontent.com/uHCnfQgxLjVpd_kq84_qG6dVNSFb-d8-pbAUk-MRrumff0cwJHQ2Xjrd15rqACkZPkPjtWo64KBbD4fbVZXTkIGmjqD1pYlVXsTKSChiTCImDLHewy_cUo72culPQF9lHCFJRvgDiGitsyFgJie0o8w)

DC  motor control with PWM & L293D

-place arduino uno and breadboard

connect power (arduino, 5V) to powerline (breadboard, bottom section)

connect ground (arduino) to groundline (breadboard, bottom section)

-connect power & ground line of the bottom secti![](https://lh5.googleusercontent.com/CiKZZCkobi8y1io4CbnbmQd1QzzAQ1E8iZ3BMdnRABvxqK5cYBUDMB8FT9EM6XD8_WDwhiAoz9dr1UUO3ves47KJiray64OZQnMmJ70vtyzou2S-URJw9KbA7YfDG0GFr0Pfg1XIhuGEc9C2LeqZwOI)on to the top section

- place L293D right in the middle of the breadboard

connect enable 1&2 to PWM 3

connect input 1 to pin 2

connect all ground to their respective powerlines lower grounds to bottom ground powerline and upper grounds  to top ground line

connect input 2 to pin 4

connect powers to their respective powerline

connect enable 3&4 to top power line

- place a dc motor ( bottom)

connect poles to input 1 and input 2( one pole = one input)

-type in code

after add 1 more motor reconnect enable 3&4 to PWM 10

connect input 3 to pin 7

connect input 4 to pin 8

connect poles to input 3 and input 4( one pole = one input)

-   rewrite code

code:

int motorlenable = 3;

int motorinput1 = 2;

int motorinput2 = 4;

 void motorforward()

{

  analogWrite(motorlenable, 127);

  digitalWrite(motorinput1, LOW);

  digitalWrite (motorinput2, HIGH);

 }

 void motorbackward()

 {

  analogWrite(motorlenable, 127);

  digitalWrite(motorinput1, HIGH);

  digitalWrite (motorinput2, LOW);

 }

void setup()

{

  Serial.begin(9600);

  pinMode(motorlenable, OUTPUT);

  pinMode(motorinput1, OUTPUT);

  pinMode(motorinput2,OUTPUT);

}

void loop()

{

  motorforward();

  delay(2000);

  motorbackward();

  delay(2000);

}

Second code:

int motorlenable1 = 3;

int motorlenable2 = 10;

int motorinput1 = 2;

int motorinput2 = 4;

int motorinput3 = 7;

int motorinput4 = 8;

 void motorforward()

{

  analogWrite(motorlenable1, 127);

  digitalWrite(motorinput1, LOW);

  digitalWrite (motorinput2, HIGH);

  analogWrite(motorlenable2, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, HIGH);

 }

 void motorbackward()

 {

  analogWrite(motorlenable1, 127);

  digitalWrite(motorinput1, HIGH);

  digitalWrite (motorinput2, LOW);

  analogWrite(motorlenable2, 127);

  digitalWrite(motorinput3, HIGH);

  digitalWrite (motorinput4, LOW);

 }

void setup()

{

  Serial.begin(9600);

  pinMode(motorlenable1, OUTPUT);

  pinMode(motorinput1, OUTPUT);

  pinMode(motorinput2, OUTPUT);

  pinMode(motorlenable2, OUTPUT);

  pinMode(motorinput3, OUTPUT);

  pinMode(motorinput4, OUTPUT);

}

void loop()

{

  motorforward();

  delay(2000);

  motorbackward();

  delay(2000);

}

mistakes

I think my dC wasnt spinnng during the first code but I cant remember the msitake

I learned to write my codes neatly today

Day 4: September 12th 2022 

objective:

introduction to 3d designing intinker cad

built a  house

get creative and built a 3d design

component:

block

cylinder

half sphere

ball

evergreen trees

text

snow covered tree

castle tower

castle tower stairway

Lesson:

-   use a mouse(the mouse scroll) to zoom in or out

-   use right click button to control angle

-   one can import 3d designs from the internet

-   download stl file because most 3d printers use stl files

built a house ![](https://lh6.googleusercontent.com/GKo0c61AVq0Xc7UuoJb3uori0XHW54urau5-3djx1JtbxTxCDvL79W1dwWpGu4YN2AyuuAdqZV8towGKypH1iBPofje5HgEcmF3Mg2AQEg90kfNX_o0whREoVCBKuAsdeii0dK0QFGk2bUJsoeOMkYM)

-place red square block then pyramid on to of it

-left click and drag over the two to select group option and adjust the measurements as one unit

-to prevent the segments from having the same color go to solid and press multicolor

- to make a chimney take out 2 cylinders, one smaller then the other in area but same height 

then group and bring over to the house, after group with the house

-   in basic shpes there is a text option this can be used to put any text youd like

get creative and make  3d design using group and cut

I went for a side of a city wall

around the house i places a wall and added a guard tower 

-   add evergreen trees within the walls add snow tree outside the wall

create a robotic arm

![](https://lh3.googleusercontent.com/e31VVRtQ3GOEVmFufx5lMZlNiVsMrPda8bsgFk8jVxNonkitbhaGWxPCcOTkWbmZWfU6-0TXzbYtjlrn6iBgX6W37pz2DNNNOpbyzCagqnxdnM4ujkXVOpRLakEyw-wUCYI0zXM5WruXSmEI8E7DOKg)

-   tke a cylinder for a part of the torso

-   -place polygon and adjust the measurements and sides

-   place ball after copy polygon 

-   then take half sphere to create the part that would grab things

-   after use a ball to create a whole

-   then place an ice cream 

-   place text and write ice cream

mistakes

sometimes i accidently shifted the objects i dint want to work on because i didnt lock them.

september

Day 5 September 13 th 2022

objective:

advise on how to correct your designs

components:

-design of house

-design of robotic arm

stl file, battery holder

lesson:

-everything has to be on scale

-every millimeter matters

robotic arm

-if the design has multiple parts it has to be printed out sepreately

-select part and export to print

-to move the parts there will have to be servo motors

- to implant servo motors the inside of the design has to be hollow

-cables will also have to fit

-note down the measurements of the design and the measurements of the servo

- make sure the design is always connected to the work plane. (height = 0.00)

house with walls

-if all parts are connected to each other one can just add a bottom layer to the design

-I can try to design the walls myself

- I can also import stuff

to import:

go to free sites with 3d files like thingi verse to download components you need

-go to thingiverse and search up component

- press download all files

-move files to download 

- go to tinkercad and press on import

- press on choose file  then press on the first file

mistakes

no mistakes

Day 6  september 14th 2022
==========================

objective:

check if the documents are correct

work on? show renewed version of your robotic arm

components

servo gear

servo mount

cover plate

bearing center bushing

gripper 120T

gripper 72T

cylinder

ball

ice cream

text

polygon

lessson

renewed robotic arm

-download gripper parts (source: Limpsquid, thingiverse)

- import all parts

- gripper measurements: scale is 1: 2.5

-align the grippers with the center bushing

- once grouped place cover plate, servo gear and servo mount

-take 3 servo mount and connect such that 3 servo mounts would fit between gripper

![](https://lh3.googleusercontent.com/wx32AMWzLkhfVF6zxCmnjwbU6Urq1dAVot3HNKo2UJpUE1TmmVtRG6thYCJ5_XPOOp8HVLgHg6PQnsqdm6SrOBbDZAlWisItyF_MnFPnvXJPvGQyVsvc0CFIAMbEECWjRhg19Ay5Ei-fztVgeqDF58M)

-group and lock

-place a cylinder and create the rotation base 

-place another cylinder on top of it

-group and lock

-place a box square and shape it into a beam

-then place cylinder and place into a disk

-then take the measurements of the servo to create the holes

-align the to so it turn into one part of the arm holder

copy it and form the holder

-group and lock

- place polygon and adjust measurements

polygon must fit between the arm holder

--place a ball then place another polygon

(the measurements must fit between the 3 servo holders

-group and lock

now connect all parts

then place text and ice cream cone

mistakes

sometimes I forgot to lock certain items and shifted the items

sometimes i forgot to unlock an item

i struggled to control the angles a little and getting all the components aligned

Day 7
=====

Objective:

-continue with dc motor control

-control the dc motors through the serial monitor. 

-learned commands:

void motorleft

void motorright 

void motorleft

review on the past 6 days

motor processor vs motor controller

motor processor: Has ability to do multiple things at one time e.g open multiple tabs at once

motor controller: Ability only allows one task? Can only run one command at once.

-void set up: Lets you set up something. Is only done once

void loop : Does the command on repeat. Is done multiple times

-variable: Name given to an object to store info

- serial.begins- the speed at which the arduino send the info over to the laptop for eaxmple

important for trouble shooting to know whats happening

-output: receice info and act on it

input: arduino receives info and reads it

pinmode: tells what mode the pin will be on on the digital pins

analogwrite (motorlenable 1,127) the speed at which the motor runs

-we did a review on the knowledge we received

Control DC motor with serial monitor

-   place arduino and breadboard

-   -place two dc motors

-   connect the dc motors as in the previous lesson

![](https://lh5.googleusercontent.com/N6Ii55ww57Lq0ySP2JvljTyXo3bKq1l-9Og0YTHoLlV_fzMBxE4GXfba-MFjX641AADVvBenjLq5s32Avs6CoN8aAx7zoEj9oe29rMBJe2I5TfzUQP2FDv1SE6grjqWplBGPX28OI4fLuDVQ95IU2VI)

-   then to the code add:

-   int state; below the other intergen

-   void motorleft with the belonging code under motor backward

-   then:  write void motorright  with the belonging code

-   lastly: write "motorstop" with the code

-   Clear void loop

-   write the if clause

Code

int motorlenable1 = 3;

int motorlenable3 = 10;

int motorinput1 = 2;

int motorinput2 = 4;

int motorinput3 = 7;

int motorinput4 = 8;

int state;

 void setup () 

{

serial.begin(9600);

pinMode(motorlenable1, OUTPUT);

pinMode(motorinput1, OUTPUT);

pinMode(motorinput2, OUTPUT);

pinMode(motorlenable3, OUTPUT);

pinMode(motorinput3, OUTPUT);

pinMode(motorinput4, OUTPUT);

}

void loop ()

{

if (Serial.available () > 0)

{

state = Serial.read();

}

if  (state  ==  "F" ) 

{

Serial,println ("Forward")

motorforward();

}

else if   (state  ==  "B" ) 

{

Serial,println ("Backward")

motorbackward();

}

else if  (state  ==  "l" ) 

{

Serial,println ("Left")

motorleft();

}

 else if (state  ==  "S" ) 

{

Serial,println ("Stop")

motorstop();

}

else 

{

Serial.println ("Input command")

}

}

Homework

read about connecting arduinouno with an ultrasonic distance sensor HC-SR04

mistakes

I didnt know I needed to clear the loop so the simulation didnt work

after I deleted that part everything turned out fine

Day 8
=====

Objective:

-connect arduino uno with ultrasonic distance sensor HC-SR04, using bread board

-connect a servo motor to this

add two DC motors

Connect Arduino with ultrasonic distance sensor HC-SR04 using breadboard

-   place arduino uno, Ultrasonic distance sensor HC-SR04, breadboard

-   Connect breadboard and arduino

-   Connect lower powerline to upper powerline. connect  VCC (Ultrasonic) to powerline connect ground (Ultrasonic) to ground powerline

-   connect trigger to PWM pin

-   connect echo to digital pin

-   write the code for the ultra sonic sensor and arduino uno

-   sent out a signal and let the serial monitor show the distance

Code (Ultrasonic sensor & arduino)

# define trigPin 3

# define echoPin2

long duration;

int distance;

void setup()

{

  pinMode(trigPin,OUTPUT);

  pinMode(echoPin, INPUT);

  Serial.begin(9600);

}

void ultra()

{

  digitalWrite(trigPin, LOW); // Wait for 1000 millisecond(s)

  delayMicroseconds(2);

  digitalWrite(trigPin, HIGH);

  delayMicroseconds(10); // Wait for 1000 millisecond(s)

  digitalWrite(trigPin, LOW);

  duration = pulseIn(echoPin, HIGH);

  distance = duration * 0.034 / 2;

  Serial.print("Distance: ");

  Serial.println(distance);

  Serial.println(" cm");

void loop()

{

 ultra();

}

Adding a servo motor

-   place a servo  motor;  

-   -connect power to powerline, ground to groundline

-   signal to PWM(Pin 5 in my case)

-   Go to code and place black slashes for the 3 lines of code 

-   below (at the beginning)

-   Serial.print("Distance: ");

-   Serial.println(distance);

-   Serial.println(" cm");

add the if clause for a distance lower than 50 turn servo 90 degrees

and for greater turn 180 degrees

added code

  if (distance < 50)

  {

   star.write(90);

   Serial.println("90");

  } 

  else if (distance > 50)

  {

    star.write(180);

    Serial.println("180");

  }

New code

# define trigPin 3

# define echoPin2

long duration;

int distance;

void setup()

{

  pinMode(trigPin,OUTPUT);

  pinMode(echoPin, INPUT);

  Serial.begin(9600);

}

void ultra()

{

  digitalWrite(trigPin, LOW); // Wait for 1000 millisecond(s)

  delayMicroseconds(2);

  digitalWrite(trigPin, HIGH);

  delayMicroseconds(10); // Wait for 1000 millisecond(s)

  digitalWrite(trigPin, LOW);

  duration = pulseIn(echoPin, HIGH);

  distance = duration * 0.034 / 2;

  Serial.print("Distance: ");

  Serial.println(distance);

  Serial.println(" cm");

void loop()

{

 ultra();

}

 if (distance < 50)

  {

   star.write(90);

   Serial.println("90");

  } 

  else if (distance > 50)

  {

    star.write(180);

    Serial.println("180");

  }

}

Mistakes 

voids like void motor right and motor left which will be called in the void loop must be written below void setup

Next homework

Add DC motor to the servomotor and ultrasonic sensor

Day 9 In Lab

objective :

-   make the circuits previously learned online physically with a partner 

-   program the circuits separately on the computer

-   make a basic blink and run the code from the arduino app to the arduino uno

-   add a push button

-   make a dimmer circuit with potentiometer

Lesson

First we downloaded 

-   arduino-1.8.15-windows

-   Ch34x_ install windows_v3_4

I partnered up with soewastika

Words learned

female: both sides of the cable dont have a wire sticking out

male: both sides of the cable have a wire sticking out

male to female: is one side has a wire the other side doesnt

Basic blink with arduino

![](https://lh3.googleusercontent.com/KYhJYRJVOX5r22AlT8mNlLOdqJNj4ahfcBsoxoXtFxexV5fX5qIQG0ewkCY_klQLdlW2-W0lSkUtAN-mfDLvsyETP37AcCrmh71BSvabSxOX_hxmQT03BU_3Dsv4f5h-fYKwIqSIh_gzbK5xRRmXamI)

-   take a red male to male cable and a black one, connect red from 5v to powerline and black from ground to ground line

-   Place LED, connect resistor from Led cathode to groundline 

connect A wire from Led anode to digital pin 2

-   Type in code, save code in folder then connect arduino to computer

-   go to tools to see if the arduino app has registered the right port 

-   upload code

mistakes

a few mistakes were made with the code because I forgot.

our first arduino didnt work

sometimes I connected to the wrong port

Led and pushbutton 

![](https://lh4.googleusercontent.com/ysJ4AiDZzptDBniC8TQLNgk4VQMKkV8qr2Q_YkFosm2wAbOXNDKasF1EENQFt13BaDzyYem86DJiFnYVWJcAdFWxYDAaONEhzx6_BLvRvaD1FFkFryCttackgSF5XLwut7Qtkmhtcy1tPb4ThpD3NXI)

-disconnect arduino from the computer

-to the previous circuit add a pushbutton ( be  careful the feet are very fragile)

- connect jumping wires to the other groundline and powerline (red and blue)

- to the right terminal of the button connect a resistor to ground

in the same column place a cable from there to digital pin 7

--  With a cable connect powerline to Left terminal (green cable)

Dimmer circuit with potentio meter

-   ![](https://lh3.googleusercontent.com/vOEj-7P5UTlw78ByWaijURzo9_Dv3Ubl7HxE4j-1f96SlFd_UtXyPrzhiYqU6tEsQojmjU4_Rd2TDaDg-M7fkzHNI2MeUcA1Q9Xlru22mnm0CZRfL_RYjSyeEUZ3ZsBfL7p7vF0dOi8qHAC1es4GsBc)

-   remove arduino from computer

-   remove all  cables for the pushbutton

-   place pot meter 

-   connect red middle of potmeter to A0 analog pin

-   connect the left side to poweline and right side to groundline

type in code

-   check port, run code check if pot meter works

Day 10
======

objective

-   learn what milli's is

-   learn why to use it

-   learn how to use it

Milli's timer in millisecond which starts the moment your arduino turn on.

Why

because it is spaghetti programming it can be very messy and takes a lot of calculating by yourself. It is used to make things more efficient.

![](https://lh5.googleusercontent.com/Y8UHmxLubeBSepWLuF646zGs-qule5RXiQHVHXaW-Q5JdpvKBzQqRbbfzwLPhBb5YBfni-DD_w03ziUFsH-5eYPzWnDqXxFDJOdW5ixHcKmApuNSvsbiOy1nX71jJ7SKZ_Uej4yWVWhSIUV4F9JRknM)

![](https://lh3.googleusercontent.com/xqNwEzRpzSO7QFpo3sDdQRSpoqrI4BPvrBmp5McGAQAEkbDvCLRgTAKzFCnifVNF4diNjruWOFEFbNzsaW6uW38ULOmQeECpX090WkoOqdkKapsd8E_VU-_4Ynp3vX3o0AHXKYRzh0MevWxB1TQemVk)

![](https://lh5.googleusercontent.com/4ZZgOCFpdixShJ696eO9YHJQM1JvBYjTrpz5hu5wmKoz5CErXWbKv73cEzNVY9-4C1wzFgKZK3reEDkI4vUtYiTPOiPBYtqibIXtQxlxzvzlQTePN2xi0aQKoJsSPj4pQrecuImhF1QjIN0iglXSM_E)

![](https://lh5.googleusercontent.com/7PdYot1ciuJPIpodlgW3VBoiUKhdSKjKebyTp2zfgeRaFLgIEcryKwWLxPWP_bCrjkQZRZgzRgnQP7H7QNoeIKvUpuzTHIANmU5g72-8IPLKsaMashseHepBC8nT569rqKmVmQBOW_GfoOixnTnPWDM)

How to use millis

-   place arduino & breadboard

-   connect powerline and groundline to arduino

-   place 3 led lights and connect to a digital pin each

-   place a resistor connecting resistor to groundline for each led

-   type in code

Code:

int redLed = 2;

int greenLed = 11;

int blueLed = 8;

int redDelay = 600;

unsigned long redLastChanged = 0;

int greenDelay = 300;

unsigned long greenLastChanged = 0;

int blueDelay = 200;

unsigned long blueLastChanged = 0;

void setup()

{

  pinMode(redLed, OUTPUT);

  pinMode(greenLed, OUTPUT);

  pinMode(blueLed, OUTPUT);

  Serial.begin(9600);

}

void loop()

{

  if(millis()- redLastChanged >= redDelay)

  {

    digitalWrite(redLed, !digitalRead(redLed));

    redLastChanged = millis();

    Serial.println(millis());

  }

  if (millis()- greenLastChanged >= greenDelay)

  {

    digitalWrite(greenLed, !digitalRead(greenLed));

    greenLastChanged = millis();

    Serial.println(millis());

  }

  if (millis()- blueLastChanged >= blueDelay)

  {

    digitalWrite(blueLed, !digitalRead(blueLed));

    blueLastChanged = millis();

    Serial.println(millis());

  }

}

Day 11

objective

-Use millis with a led and a servo motor

 - the Led must keep blinking and the servo motor needs to keep speaking

- their functions must be separate and must not interrupt each other

 components list

-- arduino uno

-breadboard

-Led

-servo motor

-resistor

Lesson

-Use internet as a source of information to find a solution

Led And servo motor Millis

![](https://lh3.googleusercontent.com/68SYRlp69-wVaK_P2AzYRp6mYAotmCs0pj7YwcKWKQ9RgJhNqpn6gNs5ZGnAnze0YioNJsbc1qhKkVTlrxZCzFwdrzabQY3tNTMYvAS6E2G3k55poZ3SYSvtm9ztri5dBbX_WbHosnfSiqLMB1yWdf0)

-take a arduino uno and a breadboard

-power the breadboard

-place led and connect cathode to the ground line

- connect Led to digital pin 2

-place servo, connect to powerline and groundline(breadboard)

if it is connected straight to arduino it will divide the voltage

coding process

start with the Led first and check if it is blinking. This will make sure you an fully focus on the servo

-start putting the normal things needed for a servo like include servo and name it

Code

#include <Servo.h>

Servo star;

int redLed = 2;

int servoPinstar = 3;

int redDelay = 200;

unsigned long redLastChanged = 0;

int starDelay = 100;

unsigned long starLastChanged = 0;

int redLedValue;

int servoAngle = 0;

void setup()

{

  star.attach(servoPinstar);

  pinMode(redLed, OUTPUT);

  Serial.begin(9600); 

}

void loop()

{

  updateRedLed();

  updateservoPinstar();

}

void updateRedLed()

{

  if (millis()- redLastChanged >= redDelay)

  {

   digitalWrite(redLed, !digitalRead(redLed));

   redLastChanged = millis();

   // Serial.println(millis());

  }

}

void updateservoPinstar()

{

  if (millis()- starLastChanged >= starDelay)

  {

  star.write(servoAngle);

  servoAngle++;

  if (servoAngle == 180) servoAngle = 0;

  starLastChanged = millis();

    //Serial.println (servoAngle++);

  }

}

-connect servomotor to pwm pin 3

mistakes

I made multiple mistakes and the thought of using the internet to my advantage to find a solution did not cross my mind. I had tried multiple codes from before Like if  clauses and mapping but it didnt give the desired result. The servo would usually turn first and then the lamp would blink. And while the Led blinked the servo would with mapping for example turn with the speed of the led but it was glitching. Later on when seeing jay's and miss julie's code I corrected and added the missing parts. It was still laginfg but the problem was fixed when turning of the serial print

DAY 12 In Lab

 objective

component list

-   arduino uno

-   servo motors

-   Led

-   breadboard

Lesson

![](https://lh4.googleusercontent.com/jxKZd154oVUH3-gskqqaY5QO82lfWUgMPmKSaEpxFBWKD2Zpx7KZZzvOqq8wIqkkoPbY4_A3Q6ZoiUKXnyQV1dMdRJHbs6a3Jw7uzeTkSde7SzZlEWC-x26_SQgcbbb8slC-dBILHzvNMRckuZCMExw)

DC motor and L293d

-   make a sketch of where to connect the wires with the L293d, DC motors and arduino

-   L293d has to be carefully placed. it is very fragile at the feet

Code

int motorlenable1 = 3;

int motorlenable3 = 10;

int motorinput1 = 2;

int motorinput2 = 4;

int motorinput3 = 7;

int motorinput4 = 8;

 int state;

void setup()

{

  Serial.begin(9600);

  pinMode(motorlenable1, OUTPUT);

  pinMode(motorinput1, OUTPUT);

  pinMode(motorinput2, OUTPUT);

  pinMode(motorlenable3, OUTPUT);

  pinMode(motorinput3, OUTPUT);

  pinMode(motorinput4, OUTPUT);

}

void motorforward()

{

  analogWrite(motorlenable1, 127);

  digitalWrite(motorinput1, LOW);

  digitalWrite (motorinput2, HIGH);

  analogWrite(motorlenable3, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, HIGH);

 }

 void motorbackward()

 {

  analogWrite(motorlenable1, 127);

  digitalWrite(motorinput1, HIGH);

  digitalWrite (motorinput2, LOW);

  analogWrite(motorlenable3, 127);

  digitalWrite(motorinput3, HIGH);

  digitalWrite (motorinput4, LOW);

 }

 void motorleft()

{

  digitalWrite(motorinput1, LOW);

  digitalWrite (motorinput2, LOW);

  analogWrite(motorlenable3, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, HIGH);

 }

 void motorright()

{

  analogWrite(motorlenable1, 127);

  digitalWrite(motorinput1, HIGH);

  digitalWrite (motorinput2, LOW);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, LOW);

 }

 void motorstop()

{

  digitalWrite(motorinput1, LOW);

  digitalWrite (motorinput2, LOW);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, LOW);

 }

void loop()

{

  if (Serial.available() > 0){

    state = Serial.read();

  }

  if (state == 'F') {

    Serial.println("Forward");

    motorforward();

  }

  else if (state == 'B') {

    Serial.println("Backward");

    motorbackward();

  }

  else if (state == 'L') {

    Serial.println("Left");

    motorleft();

  }

    else if (state == 'R') {

    Serial.println("Right");

    motorright();

    }

    else if (state== 'S') {

    Serial.println("Stop");

    motorstop();

    }

  else {

    Serial.println("Input Command");

  }

  }

DC motors and ultrasonic sensor

-   - take 4 wires, connect vcc to powerline 

-   -ground to ground line![](https://lh6.googleusercontent.com/HZoJrXQYFJBeBaE7zSOq7V3E1bCg9N8DK4Di6gA4iq19dMNabaaXPb8f8Adj5KWnMzc9uINVyhxBgsViT7oVwsBFX9ItBWhFeYaGsrFxslbD2LTu89edXqZhjLEEfWWXRLJvNIhkmW_ra9-NyipgIw0)

-   -trigger to a pwm pin and echo to a digital pin

mistakes

Since the pins are differently chosen the pins in the code differed.

when placing wires you e.g. if you want to power enable 1 if some wires are getting in the way you could place it in the same column but a row lower and it will work the same.

code

#define echoPin 12 // attach pin D2 Arduino to pin Echo oh HC-SR04

#define trigPin 11 // attach pin D3 Arduino to pin Trig oh HC-SR04

int motorenable = 3;

int motorinput1 = 2;

int motorenable2 = 9;

int motorinput2 = 4;

int motorinput3 = 8;

int motorinput4 = 7;

int state;

long duration;

int distance;

void motorforward()

{

  analogWrite(motorenable, 127);

  digitalWrite(motorinput1, LOW);

  digitalWrite(motorinput2, HIGH);

  analogWrite(motorenable2, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite(motorinput4, HIGH);

}

void motorbackwards()

{

  analogWrite(motorenable, 127);

  digitalWrite(motorinput1, HIGH);

  digitalWrite(motorinput2, LOW);

  analogWrite(motorenable2, 127);

  digitalWrite(motorinput3, HIGH);

  digitalWrite(motorinput4, LOW);

}

void left()

{

  analogWrite(motorenable, 127);

  digitalWrite(motorinput1, LOW);

  digitalWrite(motorinput2, LOW);

  analogWrite(motorenable2, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite(motorinput4, HIGH);

}

void right()

{

  analogWrite(motorenable, 127);

  digitalWrite(motorinput1, HIGH);

  digitalWrite(motorinput2, LOW);

  analogWrite(motorenable2, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite(motorinput4, LOW);

}

void motorstop()

{

  analogWrite(motorenable, 127);

  digitalWrite(motorinput1, LOW);

  digitalWrite(motorinput2, LOW);

  analogWrite(motorenable2, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite(motorinput4, LOW);

}

void ultra()

{

  // Clears the trigPin condition

  digitalWrite(trigPin, LOW);

  delayMicroseconds(2);

  // Sets the trigPin HIGH (ACTIVE) for 10 microseconds

  digitalWrite(trigPin, HIGH);

  delayMicroseconds(10);

  digitalWrite(trigPin, LOW);

  // Reads the echoPin, returns the sound wave travel time in microseconds

  duration = pulseIn(echoPin, HIGH);

  // Calculating the distance

  distance = duration * 0.034 / 2; // Speed of sound wave divided by 2 (go and back)

  // Displays the distance on the Serial Monitor

  Serial.print("Distance: ");

  Serial.print(distance);

  Serial.println(" Cm");

}

 void setup()

{

  Serial.begin(9600);

  pinMode(motorenable, OUTPUT);

  pinMode(motorinput1, OUTPUT);

  pinMode(motorinput2, OUTPUT);

  pinMode(motorenable2, OUTPUT);

  pinMode(motorinput3, OUTPUT);

  pinMode(motorinput4, OUTPUT);

  pinMode(trigPin, OUTPUT);

  pinMode(echoPin, INPUT); 

}

void loop()

//serial if statement

{

  if (Serial.available() > 0){

    state = Serial.read();

  }

//IF ELSE IF

  if (state == 'F'){

    Serial.println("Forward");

    motorforward();

    }

 else if (state == 'B'){

    Serial.println("Backward");

    motorbackwards();

    }

 else if (state == 'L'){

    Serial.println("Left");

    left();

    }

 else if (state == 'R'){

    Serial.println("Right");

    right();

    }

 else if (state == 'S'){

    Serial.println("Stop");

    motorstop();

    }

 else{

    Serial.println("Input Command");

    ultra();

 }

  }

DC motor with bluetooth HC-05

![](https://lh5.googleusercontent.com/d-VofdA61qPOgijvSrZTcukTR_5zqnHgOXLIUgtWHT6tzRWjt64-mu58CR-x68U_O88rQ6GWN2RK7r_nuOCdd8D3-47EPYlls1DXwN56z0iSpcstCquk_oPUq819xIph0GnKdekd2Ip9cu121aML6-k)

![](https://lh6.googleusercontent.com/Np-oOE_pyEESYQ6rZFe2oQUJN7aC9OUUvhoetVOCGSw_if_NYbrMFjCLrLRaGtWn04mbN60KkRJ88bSY8li7HLF4zERLEV2TluILY0Kt_tXGj1yHQ8o45DRSqEZPax2DOBNVm1Gs8UUyH6X0Pp7d5Z0)

-this app must be downloaded to control the robot via bluetooth

-connect tx to rxd and rx to txd, connect vdc to powerline and ground to ground

mistakes

we were having some problems with connecting for some reason

Day 13 Piezo

Objective:

-wire and code a piezo

- make it play the piezo play a tune

Components list

-Arduino uno R3

-breadboard

-piezo

Piezo

-  I searched online how to wire and code a piezo

- I took a breadboard and an arduino and a piezo

Code

int buzzer = 3;

void setup() 

{

    // Defines the Buzzer pin as output 

    pinMode(buzzer,OUTPUT);    

}

void loop() 

{

    // Sounds the buzzer at the frequency relative to the note C in Hz

    tone(buzzer,261);    

    // Waits some time to turn off

    delay(200);

    //Turns the buzzer off

    noTone(buzzer); 

    // Sounds the buzzer at the frequency relative to the note D in Hz   

    tone(buzzer,293);             

    delay(200);    

    noTone(buzzer); 

    // Sounds the buzzer at the frequency relative to the note E in Hz

    tone(buzzer,329);      

    delay(200);

    noTone(buzzer);     

    // Sounds the buzzer at the frequency relative to the note F in Hz

    tone(buzzer,349);    

    delay(200);    

    noTone(buzzer); 

    // Sounds the buzzer at the frequency relative to the note G in Hz

    tone(buzzer,392);            

    delay(200);

    noTone(buzzer); 

}

mistakes

I struggled a bit to understand how the codes worked because of the overload of information on line and I didnt know where to start. I didnt know that everynote has a frequency

Day 14

Objective:

-   wire the two motors to the motor driver L298n, an arduino nano and a battery holder.

Component list:

-   L298N

-   arduino nao 

-   wires

-   batteries

-   battery holder

code

int motorlenable1 = 9;

int motorlenable3 = 3;

int motorinput1 = 8;

int motorinput2 = 7;

int motorinput3 = 5;

int motorinput4 = 4;

int state;

void setup()

{Serial.begin(9600);

  pinMode(motorlenable1, OUTPUT);

  pinMode(motorinput1, OUTPUT);

  pinMode(motorinput2, OUTPUT);

  pinMode(motorlenable3, OUTPUT);

  pinMode(motorinput3, OUTPUT);

  pinMode(motorinput4, OUTPUT);

  Serial.println("Input your command: F=forward, B=backward,L=left,R=right, S=Stop");

}

void motorforward()

{

  analogWrite(motorlenable1, 127);

  digitalWrite(motorinput1, LOW);

  digitalWrite (motorinput2, HIGH);

  analogWrite(motorlenable3, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, HIGH);

 }

 void motorbackward()

 {

  analogWrite(motorlenable1, 127);

  digitalWrite(motorinput1, HIGH);

  digitalWrite (motorinput2, LOW);

  analogWrite(motorlenable3, 127);

  digitalWrite(motorinput3, HIGH);

  digitalWrite (motorinput4, LOW);

 }

 void motorleft()

{

  digitalWrite(motorinput1, LOW);

  digitalWrite (motorinput2, LOW);

  analogWrite(motorlenable3, 127);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, HIGH);

 }

 void motorright()

{

  analogWrite(motorlenable1, 127);

  digitalWrite(motorinput1, HIGH);

  digitalWrite (motorinput2, LOW);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, LOW);

 }

 void motorstop()

{

  digitalWrite(motorinput1, LOW);

  digitalWrite (motorinput2, LOW);

  digitalWrite(motorinput3, LOW);

  digitalWrite (motorinput4, LOW);

 }

void loop()

{

  if (Serial.available() > 0){

    state = Serial.read();

  }

  if (state == 'F') {

    Serial.println("Forward");

    motorforward();

  }

  else if (state == 'B') {

    Serial.println("Backward");

    motorbackward();

  }

  else if (state == 'L') {

    Serial.println("Left");

    motorleft();

  }

    else if (state == 'R') {

    Serial.println("Right");

    motorright();

    }

    else if (state== 'S') {

    Serial.println("Stop");

    motorstop();

    }

  else if (state == '?'){

    Serial.println("Input your command: F=forward, B=backward,L=left,R=right, S=Stop");

  }

  }

 mistakes

sometimes we turned the screw in the wrong directions sometimes.

Day 15

Objective:

Today we decided on what we wanted to design for our project and then also learned about maze

-   understand how a distance sensor works

Components list: _

Coding:-

mistakes: None. However I didnt completely understand the maze code.

Day 16

Objective: Start on our final project

Component list: -----

Lesson: There wasnt really a lesson since we had to start designing. We did more research today because we had little idea on how to make an air cooler

Mistakes: ---------------------

Day 17

Objective: Work on assembling the base of the rover.

![](https://lh6.googleusercontent.com/GNkMrRNZyr6FSu26WvGb1VltCJ0kaL1KE7FcGTrZ4_vBUlXkgBVOdy9MZL1wyEok_aKxlAo_SrFpO0fuk7uSQ8G_y9xorRPfwx_QNemlKTO4WWWvcimcfDWyf1oIz3jJ6nhdZGhIvarbEdaK9hnVe2E)

 component List:

Box

motor driver

Dc motor

Arduino nano

Wires

Servo motor

Day 18

Objective: make the circuit for the extra feature. We only have a fan.

Components list: 

Led 

Arduino uno

Breadboard

Slide switch

resistor

Hands on

![](https://lh4.googleusercontent.com/TEUTAZOXEYpz5ZshTcaG1pYaOfRSdgpI1pWdFOn80UVzcEIWvmsW2ANK8r6BRZWN5_8X39R3pmeCcLhY4-GsiK-mEFHTJYicyfo7Tq4JkMGkO230P12wLW_KU9BEyVzqOsf7CC1epwzL8DvYHHZXTYI)

The led is supposed to represent the fan

Mistakes:  At first I didnt understand what I needed to do but I understood later. I forgot how to make a basic blink

Code:

Day 19

Our objective today was to get our fan to work

Components list :

Same as last time

-   battery pack

-   fan * 2

Hands on

We added our battery pack. Then we got our fan After searching on the internet we tried it out. And the fan spun!![](https://lh4.googleusercontent.com/uW2LirYESxG2YmknLkeFtclRYK3m1BVej2BrXRrLteCncgN4bapS5YXkcgeivfRGtHJt_cm5j2Joyo88Vf7OcD0Zr6AA9dC6baWzl4reDrpf-KiB9VYo7VNj2JEQIYCsffaNF1oePdA_j_VF_cnnT8g)

One of the wheels werent spinning correctly so we had to switch the cables

mistakes. I accidentally broke on of the cables of the servo motor so it had to be unscrewed and soldered

DAY 20

Today we didnt do much. It was a support session.

Day 21

Objective Our objective was to make our second fan spin

Componets list:

Same as last time

Hands on

The fan didnt spin because we dont have enough power

Day 22

 8 november 2022

 Objectice: Finish documentating Our documents

Make a 3d version in tinkercad

components list: none

Mistakes: no mistakes made.

Day 23: 11 november 2022

Objective:

My objective today was to transfer my rover unto the plastic box.

I also started working on creating the fan.

component list:

  -- same as "day 21"

       +

- plastic container

- old hair conditioner container

- stiftpen (for drawing where to drill)

hands on

make holes in the container

(I used an <according to miss julie, dull rasper)\
![](https://lh6.googleusercontent.com/3O1ajbJqeJfKI6vJe2RU1mry3CG02YvJpWTpa45i48OsLzNsHo9PaWIWR829qAQES5AeUNXrEyJvg4WP8vnLuiLphbyvLNaAZwUF82C4gPbJ8q2AgBjbuIFJRnOTsa3jdDMiy9plIeMk-l4eNEOJuYE)

1.  two wholes on top of the     container

2.  one for the wires of the fan to pass through

3.  one for the servo motor and cables of the servo motor to pass through\
![](https://lh3.googleusercontent.com/Ri2zXURKnYWejOuRepdt8r9wRO-lQtAmD_qX8_esdaNgkumvV8sAs2t_HF-HqHBeHpc4lgxsHvZk7UJDCmYtRLjWaMefh1lImGBNcdWDP59L9GofJDUKsGkbWZNb1m2sIaQty1pCiRgVjgwJXUr3KG0)

-   make a hole for the wires of the battery pack to pass through

-   make a whole for the wheels of the rover each.

![](https://lh3.googleusercontent.com/wc1-jfyMseRcxGdlwtZLurfigTj4Y0Ns41qWCGaQ_qImM9tuKmMckb0cN8P-v4NZEZO0hpL7TpDSRsUtq5nndRySGW9BpUyTofQPkH1SLe_iJqGXqAVq723T2m9pM0SPAu07o02piFqfWie5oclslPA)

![](https://lh6.googleusercontent.com/CCqlBJFoDtDd8eYvnGprXuF0xpZF7Lh_ofOfwoErBMEEDmHRyNBD3tzWzXksyuxL2N4xUKKoWDhLAg-dZg65gi8jbIluNK9Tw4i1RJO5PvpxiOyRlbEH29RCPjoh-200h4JcFNuJG78PVi_Bpzw-0Bc)

the aircooler
=============

-   the fan surprisingly worked before

-   make 3 holes on top of the empty hair conditioner container  so the ends of the fan can fit. (ignore the smallest one).

-   make one big hole (this was done with a heated iron pipe) for the fan to suck air.

-   ![](https://lh5.googleusercontent.com/baPld98_3WTkOyaQRU4YXBJNQWDNushP6e5eIp_aNFqzXp6b150xQVCUX6zhQUWA5BzIExQRTBVWUQYlPsTKx7aSAazsWx1e8fWbkFU_imn-woIFqW1rBi67wGmlhHhNJcS8foMbgqp5ww6K9qASrRg)

-   ![](https://lh6.googleusercontent.com/n-UZWxHCR08Xr04aaCDl2TJhrihv85UDYSfll3vbz9XdwGOIaunBD1YM7l5MjKkiBMwmWVm3g2uX4KkAsyshCaHx2dRvYWb9FK0chn8jXCpFbz3-zLsJcHfXdPwhxipfu4U01MS4N4NKECgN8UNLLUc)

-   make one big hole for the air to go out. This was done using a iron pipe![](https://lh4.googleusercontent.com/mlw1P-RuEK1Vq5Dn56KW4h5ZprzbbNuHz5SqJXznSc5WKZ68Rp8ROatswAI5NbkXQsKOjhLBXvxGwLcJGofXm87CUVGoQT9mm_f-54bLP5A1Hk_rKtlSR4F3xX894FDv2kLGAq-AGGMRBbomG9Y_g6U)

-   make a  whole for the  wires of the fan to go out![](https://lh6.googleusercontent.com/dtovTWxRCcnbzcH1AQZ43wg9hh-wU4VcljnRFK35y7q1hWhD23BYmS6OTfnX1TIpscS8kdgMHl22Z3GPynQxZb2qnDP3pusZcxz1VmopcFkDKoQmI8LdPHwOhOOxLUEeCgIBRsQFLkTrDbOvE53TjKE)

-   Now you have the fan with the fan container

Extra day at the lab: 13 november 2022

Dylan showed me how to make an n gate so that my fan could get higher power

note: fan pin wont work if one of the 3 pins is missing.

![](https://lh6.googleusercontent.com/qkGT3vwzr5pN5FVA33Ld0XorC00QTs8o6PY0B5wxfj-766HWmDc_TI9sKXcKUgHo2g0rQIAJ385kYEEzB8aJn5KON1-fvM7PRgTMlUhg9YodQ9kN_ZvDrDhA0BsEogsJJb5JVcU09lLwTarO8N-yMh4)

![](https://lh5.googleusercontent.com/Z8FqSlisRqW64Kbzt6K2C2h-PDqAJCG4WwicJtKxYx4yUA-fywdlv1uYujVylyPVzdY1higbftZ_xrHcdP0Zn1oyTbDIibw0W67lyT5WisYeZSifshiZFa5-FL7FibfkC5g29NpRgvb_4Dl-mjX2qu8)

Day 24: 18 november 2022

Objective:

  My objective today was to:

-   change the DC motor with a cut cable

-   finish all the circuits

components list:

 same as last time

Hands on

I transferred everything to the bread board with the transistors

-   one power rail is 12v and the other is 5v

-   note to self: do not mix up the two rails

-   we switched the dc motor cause one of them broke again.

mistake 

we almost burned the  arduino nano because I connected the ground to power and power to ground on the 5v power rail. It hurt.

there mightve been the a loose connection because one of the DC motors wouldnt spin

Day 25 
=======

objective:

Fix Dc motors and test codes

Components list:

everything on previous components list 

+

relay

Hands on

After fixing the dc motors. we wired it back to the circuit and checked if everything was working. Fan, buzzer, motor, servo motor and distance sensor. I asked either mr theo or miss julie if a bigger battery pack could be made because My fan was blowing very softly.

It would be possible but it would mess with the motors. So he taught us how to use a relay instead. Because the cpu has 3 wires. We decided to hard wire it. That means that it would just be on or off.Because the signal pin would be connected to the power pin.This would let the fan spin a bit faster without having to add more batteries.

DAY 26
======

Objective:

-   figure out how to work with a relay

-   try to build the circuit

hands on

I forgot to do research on  the relay. So mr theo let us research on line on how to use it and how to wire it to the fan and the rest of the circuit.

after some tries mr theo helped us and explained how to wire it. The relay was clicking but the fan still wasnt spinning. Mr theo told me to check at home what exactly the problem was. However the wiring for the relay was correct. So I needed to figure out what the problem was exactly.

DAY 27
======

objective: 

-finish wiring relay with fan

- figure out why maze isnt working

hands on

the relay was working. There seems to be a loose conection in the cables sometimes.

problem with maze. Maze wasnt working properly so I broke up the codes into different parts to check where the mistakes lay. And slowly added them up again to see what the problem was.

The dc motors spinned on in one of the codes but didnt want to with the maze code. Later I found that the moment star.attach was written into the code the dc motor would stop working or only one worked. I used a volt meter to see what the problem was.

It seemed that the moment star.attach was written out 1 and out 2 on the motordriver stopped receiving electricity. This happened because pin 9 stops being a pwm pin after the servo library is added. And the pin needed to be a pwm pin for the motor to drive. Since our fan was on a pwm pin we switched the pins for the fan and motor.

DAY 28
======

objective:

-   rewrite maze code

-   practice speech for graduation 

-   make a google slide

Hands on

I forgot my laptop so me and my partner had to rewrite the maze code and get it to work. We also glued the Aircooler to the rover so it wont cause problemsin the future.

We practiced what we were gonna say for when we graduate. What we learned and how are experience was in codettes.

miss julie told us to make a google slide of us working on our project.

mistakes

our speech was a bit too long

I forgot my laptop

Day 29
======

Objective:

Record video for what we've learnt during the program

Finish google slide

finish 3d design of our mobile rover

Hands on

Today we tested if the bluetooth module still works. We checked if everything was set on bluetooth electronics. I added to more buttons for the fan.

I was working on my google slide and my partner was working n the 3d design. 

Miss julie recorded us on everything we did, learned, how ur experience was and what mistakes we made.

![](https://lh4.googleusercontent.com/xHp9AerV84VHr1838K3DejW66FcjIf-OGQ6STkAoBknFB6WLKh5EtWgDG08lGbUXwv5T2QzCfa4_6QFECZpfhFUJ6a_J3qrNS5YljBKiwTdma8JQmbZbTF1_6x8ZzaZZfFXj0FejQQ5vBxU8AFbanF8)