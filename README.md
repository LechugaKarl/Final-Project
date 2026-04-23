# Final Project
Steps and Procedures
<details>
<summary>RC Car using Esp32-D and L298N Motor Driver</summary>

INTRODUCTION:

In the rapidly evolving field of embedded systems and robotics, the development of remote-controlled (RC) vehicles serves as a fundamental benchmark for integrating hardware control with wireless communication. This project focuses on the design and implementation of an RC car powered by an ESP32 microcontroller and controlled via an L298N motor driver module.

The system leverages the computational efficiency of the ESP32 to process control signals—transmitted wirelessly via Wi-Fi or Bluetooth—and translate them into precise mechanical movements. Because microcontrollers operate at low voltage and current levels, they cannot directly drive the high-power requirements of DC motors. This is where the L298N motor driver acts as a critical interface, functioning as an H-Bridge to allow the ESP32 to control the direction and speed of the wheels through Pulse Width Modulation (PWM) and digital logic switching.

_______________________________________________________________________________________________________________________________________________________________________________________________________________________

<details>
<summary>COMPONENTS</summary>

ESP32-D
The ESP32-D (specifically the ESP32-D0WD series) is a powerful, dual-core system-on-a-chip (SoC) designed by Espressif Systems. It is the core processor used in many popular ESP32 development boards and is tailored for high-performance Internet of Things (IoT) applications that require both Wi-Fi and Bluetooth connectivity.

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/esp32D.jpg)

PINOUT:

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/esp32DA.jpg)
_______________________________________________________________________________________________________________________________________________________________________________________________________________________

L298N Motor Driver
The L298N is a high-power, dual H-Bridge motor driver module commonly used to control the speed and direction of DC motors and stepper motors.
Since microcontrollers like the ESP32 or Arduino cannot provide enough current to spin motors directly—and could be damaged if they tried—the L298N acts as a heavy-duty switch between a high-voltage battery and the motors.

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/l23d.jpg)

PINOUT:

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/l293dA.jpg)
_______________________________________________________________________________________________________________________________________________________________________________________________________________________

DC Motor
A Direct Current (DC) motor is an electrical machine that converts electrical energy into mechanical energy. It operates on the principle of Lorentz Force, which states that when a current-carrying conductor is placed in a magnetic field, it experiences a physical force that causes it to move.

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/dc%20motor.jpg)

_______________________________________________________________________________________________________________________________________________________________________________________________________________________

Lithium Ion Battery
A Lithium-ion (Li-ion) battery is a type of rechargeable battery that relies on the movement of lithium ions between a positive electrode (cathode) and a negative electrode (anode) to store and release energy.
Because of their high energy density and light weight, they are the standard power source for modern portable electronics, electric vehicles, and—most relevantly—high-performance robotics projects like your RC car.

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/Battery.jpg)

_______________________________________________________________________________________________________________________________________________________________________________________________________________________

<details>
<summary>SCHEMATIC DIAGRAM</summary>

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/a.jpg)

_______________________________________________________________________________________________________________________________________________________________________________________________________________________

<details>
<summary>CODES</summary>

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/code1.jpg)

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/code2.jpg)

![Image Alt](https://github.com/LechugaKarl/Final-Project/blob/main/assets/code3.jpg)

_______________________________________________________________________________________________________________________________________________________________________________________________________________________

SAMPLE VIDEO
https://github.com/user-attachments/assets/89fd2ed1-6db1-4794-8f57-b2e1660d32ae
________________________________________________________________________________________________________________________________________________________________________________________________________________________

<details>
<summary>CONCLUSION</summary>
The successful construction of the RC car demonstrates the effective integration of high-level wireless processing with low-level power electronics. By utilizing the ESP32-D, the project moved beyond traditional radio control into the realm of IoT (Internet of Things), proving that dual-core microcontrollers can simultaneously manage complex Wi-Fi/Bluetooth communication stacks without interrupting the real-time PWM signals required for motor stability.
The implementation of the L298N Motor Driver served as a critical lesson in power management and isolation. It successfully bridged the 3.3V logic of the ESP32 to the higher voltage demands of the DC motors, while the use of Lithium-ion batteries provided the necessary energy density to maintain consistent torque and speed.
Ultimately, this project confirms that a modular approach—separating the "brain" (ESP32), the "muscle" (L298N), and the "power" (Li-ion)—is an efficient architecture for robotics. The skills developed here in circuit design, code optimization, and wireless interfacing provide a robust foundation for more advanced engineering applications, such as autonomous navigation or sensor-based waste classification systems.
