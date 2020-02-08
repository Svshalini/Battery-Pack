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
 |Hardware              |Description                                                                     |
 |----------------------|--------------------------------------------------------------------------------|
 |MicroController       | [STM32F446RET6](https://www.st.com/resource/en/datasheet/stm32f446re.pdf) Arm® Cortex®-M4 32-bit RISC core @ 24MHz,512 KB flash,128 KB SRAM|
 |CAN transceiver       |[TJA1050](https://www.nxp.com/docs/en/data-sheet/TJA1050.pdf)                   |
 |Tamper Sensor         |Light Dependant Resistor                                                        |
 | Battery Guage Meter  |[BQ34Z100-G1](http://www.ti.com/lit/ds/symlink/bq34z100-g1.pdf)                 |
 
## Tool chain
|Tool                  |Description   |
|----------------------|--------------|
|IAR Embedded Workbench|version 8.40.1|
|STM32 CubeMX          |version 5.4   |

## Description
* Battery ID Labelling Scheme
     
     * Battery pack [ID](https://racenergy-my.sharepoint.com/:x:/g/personal/arun_racenergy_in/EYIPOkjBp4xKjgCBu79ZSjoB2fk5onWlVYXAaaI0KpPx1Q?e=Cskpca&CID=2b26a81f-2f6f-44f4-7043-d1a0a568732b) - [RACE][A][03][A][001]
       |Label |Descriptor          |Range   |Example  |
       |------|--------------------|--------|---------|
       | RACE |Complany Name       |-       |RACEnergy|      
       |  A   |Year                | onwards| 2019    |
       |  03  |Batch number        |01-99   | 03      |
       |  A   | Pack Configuration |        |14S, 11P |
       |  001 | Serial Number      |001-999 |001      |
 
* **Battery Gauge Meter** 
    * SoC estimation using impedance track method.
      * SoC(State of Charge) is the level of charge of an electric battery relative to its capacity.
      * It is the level of charge of an electric battery relative to its capacity. Percentage is the units of SoC.
    * Supports I2C interfacewith normal current consumption 145μA-average current
    * [DATASHEET](http://www.ti.com/lit/ds/symlink/bq34z100-g1.pdf) can be found here. 
    
* **BMS** 
    * It is an electronic system that manages rechargable battery(cell or battery pack), monitoring it's state, protecting the battery from operating outside it's safe operation area.
    * A battery management system is essentially the “brain” of a battery pack; it measures and reports crucial information for the operation of the battery and also also protects the battery from damage in a wide range of operating conditions. 
    
