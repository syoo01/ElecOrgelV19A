# ElecOrgelV19A
Electric Music Box project begin 2019 January 2nd at Seoul  

Parts/Components
A-1 : Arduino Nano
A-2 : RTC module DS1307
A-3 : 4 digit LED with Driver module (TM1637Z)
A-4 : 4 push button Switch for Set Alarm Time
A-5 : Electric Orgel Module with Electic Motor (1.5V)

Connection To Arduino Nano
DS1307 : A4(SDA), A5(SCL)
TM1637 : D2(CLK), D3(DIO)
Switch : D4 (Mode), D5(Hour), D6(Minute), D7(Reset)
Motor  : D11 (Buck Converter revered - FF(0V), 00 (5V)) 

needed Libraries
DS1307 - RTClib
TM1637 - Digital Tube
Switch - Timer0ne
Motor  - TimerOne

Resource usage 
Timer 0 - default
Timer 1 - Time check 
Timer 2 - PWM for Motor Driver

Interrupt - Timer 1 

User Control
Time Set : Mode (Run / Set Alarm) 
