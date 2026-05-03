 Embedded EV Battery Management System (BMS) Using STM32 and LTC6811 with Real-Time Monitoring & Data Logging

This project presents the design and development of an embedded Battery Management System (BMS) for electric vehicle (EV) applications. The system is based on the STM32 Microcontroller and the LTC6811 Battery Stack Monitor for accurate multi-cell voltage measurement, temperature monitoring, and system protection.

The BMS is designed to:

 Monitor cell voltages
 Measure pack current
 Track battery temperature
 Provide real-time data logging
 Ensure safe operation under different conditions

System Architecture
![Block Diagram](docs/images/bms-system-block-diagram.png)

The system consists of:

 Battery model (Simulink)
 Sensors (voltage, current, temperature)
 SOC estimation block
 Protection logic (Stateflow)
 Data logging system
 
 Output Results
![Output Graph](docs/images/bms-output-graph.png)

The simulation results show

 Stable pack voltage behavior
 Dynamic charge/discharge current response
 Controlled temperature variation
 
 Hardware Components

 STM32 Microcontroller
 LTC6811 Battery Monitoring IC
 Temperature Sensors
 Current Sensor
 Data Logging Interface (SD Card / Serial)
  
 Features

 Real-time battery monitoring
 Multi-cell voltage measurement
 Safety protection (overvoltage, overcurrent, temperature limits)
 Simulation + hardware approach
Data logging and visualization

Repository Structure

bash
/Firmware        # STM32 embedded code (if available)
/Hardware        # PCB design and schematics
/docs/images     # Diagrams and output graphs

 Testing & Validation

 Simulated charge/discharge cycles in Simulink
 Monitored voltage, current, and temperature behavior
Verified system response under varying load conditions

Future Improvements

 Integration of FreeRTOS for real-time task scheduling
 Implementation of State of Charge (SOC) estimation
 Addition of State of Health (SOH) prediction
 CAN communication for EV system integration
 
Conclusion
This project demonstrates a complete embedded BMS design combining simulation hardware architecture and real-time monitoring It provides a solid foundation for further development in advanced battery management and EV systems.

