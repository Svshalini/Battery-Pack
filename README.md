# Battery Pack

## Features
- [ ] Unique Battery ID
- [ ] CAN 2.0B Network - 500Kbps
- [ ] Tamper Sensors
- [ ] Over Temperature Protection
- [ ] RCPS with Charge Inhibition
- [ ] BMS - Battery Management System

## Hardware used
 |Hardware <?dbfo bgcolor="dark brown"?>             |Description <?dbfo bgcolor="dark brown"?>|
 |---|---|
 |MicroController       | STM32F446RET6 Arm® Cortex®-M4 32-bit RISC core @ 512 KB flash,128 KB SRAM|
 |CAN transceiver       |TJA1050|
 |Tamper Sensor         |Light Dependant Resistor|
 | Battery Guage Meter  |BQ34Z100-G1|
 
## Tool chain
|Tool <?dbfo bgcolor="dark brown"?>|Description <?dbfo bgcolor="dark brown"?>|
|---|---|
|IAR Embedded Workbench|version 8.40.1|
|STM32 CubeMX|version 5.4|

## Description
* Battery ID LABELLING SCHEME
     
     * ID - [RACE][A][03][A][001]
       1.  RACE - RACEnergy             
       2.  A - year(2019)
       3.  03 - Batch number(3)
       4.  A - Pack Configuration ( 11P)
       5.  001 - Serial Number
 
* Battery Guage Meter 
    * Capacity estimation using impedance track method 
    * It supports I2C interface.
    * You can find more about this here. [DATASHEET](http://www.ti.com/lit/ds/symlink/bq34z100-g1.pdf)
    
* BMS :
       It is an electronic system that manages rechargble battery(cell or battery pack), monitoring it's state, protecting the battery from operating outside ot's safe operation area.
* Soc(State of Charge) :
It is the level of charge of an electric battery relative to its capacity. Percentage is the units of Soc. Soc of attery pack is equivalent to fuel gauge. 

## Block Diagram
![image](https://github.com/vatsava-rac/Battery_Pack/blob/master/Docs/block%20diagram/battery_blockdiagram_v_1_2.jpg)
