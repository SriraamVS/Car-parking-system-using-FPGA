# Car-parking-system-using-FPGA

**Abstract**
    The project aims to develop a car parking system using VHDL, which enables the control and guidance of the parking process. The system is composed of an identification module and two sensors (front and back) to detect the presence of a car. The identification module allows access to the parking slot only with the correct security key (password). The system utilizes VHDL to control the sensors, identification module, and parking slots. The implementation of the car parking system using VHDL provides a reliable and efficient solution for controlling and managing parking slots. 

**Introduction**

    In modern times, the frequent use of motor vehicles has led to problems like traffic congestion, pollution, and parking difficulties. To tackle these issues, a Parking System based on Finite State Machine (FSM) and VHDL language has been proposed. The system consists of two sensors, front and back sensors, along with an identification module that requires a security key or password to park the vehicle. This module ensures the safety of the parking system by permitting only authorized users to park their vehicles in the designated slots. By implementing a systematic parking approach with appropriate security measures, the proposed system guarantees a safe and efficient parking experience, with minimal risk of accidents or collisions. They serve advantages like saving space, time and fuel as one does not have to drive around for finding empty space.

**Flow chart**
    • IDLE: Initially, the FSM remains in the idle state. When the front sensor detects a car, 
    the FSM moves to the next state.
    
    • WAIT_PASSWORD: The FSM moves to the wait password state upon detecting a 
    car. In this state, the driver enters a password. If the password is correct, the gate opens, 
    and the car is permitted to enter the parking zone. The FSM indicates the right password 
    by expressing RIGHT_PASS and blinking the Green LED.
    
    • WRONG_PASSWORD: If the driver inputs an incorrect password, the FSM shifts to 
    the wrong password state and flashes the Red LED. The driver is required to re-enter 
    the password until it is correct.
    
    • STOP: Upon detecting a car entering the parking zone, the back sensor identifies it. If 
    another car approaches, the FSM moves to the stop state and flashes the Red LED. The 
    Red LED blinks to signal the following car to stop and input the password. After the 
    car enters the parking zone, the FSM returns to the IDLE state.
