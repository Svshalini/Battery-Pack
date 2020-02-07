# Battery_Pack

## Features

- [ ] Unique Battery ID
- [ ] CAN 2.0B Network
- [ ] Tamper Sensors
- [ ] Over Temperature Protection
- [ ] RCPS with Charge Inhibition

## Hardware Used
 |MicroController       | STM32F446RET6 medium-density Arm® Cortex®-M4 32-bit RISC core @180MHz, 512 KB flash,128 KB SRAM|
 |CAN transceiver       |(1)TJA1050, (2) Sn65hvd233|
 |Tamper Sensor         |Light Dependant Resitor|
 | Battery Guage Meter  |BQ34Z100 G1
  
## Description
* Battery ID LABELLING SCHEME
     
     * ID - RACEA03A001
       1.  RACE - RACEnergy             
       2.  A - year(2019)
       3.  03 - Batch number(3)
       4.  A - Pack Configuration ( 11P)
       5.  001 - Serial Number
 
* Battery Guage Meter
    * Capacity estimation using impedance track method for batteries from 3V to 65V
    * Supports battery capacities upto 29Ah, charge and discharge currents upto 32A
                 
