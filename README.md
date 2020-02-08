# Battery Pack

## Block Diagram
![image](https://github.com/vatsava-rac/Battery_Pack/blob/master/Docs/block%20diagram/battery_blockdiagram_v_1_2.jpg)

## Features
- [ ] Unique Battery ID
- [ ] CAN 2.0B Network - 500Kbps
- [ ] Tamper Sensors
- [ ] Over Temperature Protection
- [ ] RCPS with Charge Inhibition
- [ ] BMS - Battery Management System

## Hardware used
 |Hardware              |Description|
 |---|---|
 |MicroController       | STM32F446RET6 Arm® Cortex®-M4 32-bit RISC core @ 24MHz,512 KB flash,128 KB SRAM|
 |CAN transceiver       |TJA1050|
 |Tamper Sensor         |Light Dependant Resistor|
 | Battery Guage Meter  |BQ34Z100-G1|
 
## Tool chain
|Tool                  |Description|
|---|---|
|IAR Embedded Workbench|version 8.40.1|
|STM32 CubeMX          |version 5.4|

## Description
* Battery ID Labelling Scheme
     
     * ID - [RACE][A][03][A][001]
       |||
       |---|---|
       | RACE | RACEnergy   |          
       |  A | year(2019)|
       |  03 | Batch number(3)|
       |  A | Pack Configuration ( 11P)|
       |  001 | Serial Number|
 
* **Battery Gauge Meter** 
    * Capacity estimation using impedance track method 
    * It supports I2C interface.
    * [DATASHEET](http://www.ti.com/lit/ds/symlink/bq34z100-g1.pdf) can be found here. 
    
* **BMS** 
    * It is an electronic system that manages rechargable battery(cell or battery pack), monitoring it's state, protecting the battery from operating outside it's safe operation area.
    * A battery management system is essentially the “brain” of a battery pack; it measures and reports crucial information for the operation of the battery and also also protects the battery from damage in a wide range of operating conditions. 
    
* **SoC**(State of Charge) 
    *  It is the level of charge of an electric battery relative to its capacity.
    *  Percentage is the units of Soc.
