# Temprature-Controlled-DC-Fan-Using-Lm741 🌡️🌀
Developing a temperature-controlled DC fan using an **_LM741 Op_** amp and an **_NTC thermistor_** to regulate the bedroom temperature sounds like a promising project to improve sleep quality for people with insomnia.<br><br>

The **_primary objective_** of this project is to develop a cost-effective and adaptable temperature control system using a temperature-sensitive sensor (NTC thermistor) and an operational amplifier (LM741). By accurately monitoring the ambient temperature, this system will automatically activate or deactivate a DC fan to achieve and maintain the desired temperature setpoint. The key goals of this project include:
## Components Required 🛠️
- **NTC Thermistor:** 
   - An NTC (Negative Temperature Coefficient) thermistor is a temperature-sensitive resistor whose resistance decreases as the temperature increases. You'll need this to measure the bedroom temperature
- **LM741 Op-Amp:**
   - The LM741 is a commonly used operational amplifier that can be configured to amplify the voltage difference between the NTC thermistor and a reference voltage to control the fan.
- **DC Fan:**
   -  Choose a DC fan suitable for the size of the room and the desired airflow. Ensure that it can be easily powered and controlled.
- **Power Supply:**
   - You'll need a suitable power supply for the fan and the op-amp circuit. Make sure it can provide the required voltage and current. 
- **Resistors and Capacitors:**
   - You may need resistors and capacitors to set up the op-amp circuit and to filter any noise.
- **1N4007 Diode:**
   - The 1N4007 diode can be used for flyback protection when controlling inductive loads like DC fans. When the fan is turned off, the collapsing magnetic field can induce a voltage spike that could potentially damage the circuit. The diode, when connected in parallel with the fan, allows this voltage to safely dissipate.
- **BD140 Transistor:**
  - The BD140 is a PNP transistor that can be used as a switch to control the power supply to the DC fan. It amplifies the current from the LM741 op-amp to drive the fan effectively.

## Circuit Diagram: 🗺️ 
 ![image](https://github.com/Drupad-DeV/Temprature-Controlled-DC-Fan-Using-Lm741/assets/100958162/223dce5c-bad5-4f8c-b556-27dd849e36b7)
 <br><br>
 Circuit Schematic At LTSpice
![image](https://github.com/Drupad-DeV/Temprature-Controlled-DC-Fan-Using-Lm741/assets/100958162/20cfac46-4689-4d0a-ac32-b383aacb7d9e)

## Circuit Working: 🔄
The Circuit Design is simple, Negative temperature coefficient (NTC) Thermistor decreases its resistance when the temperature increases while Positive temperature coefficient (PTC) increases its resistance when the temperature increases. Here a 4.7K NTC Thermistor is used, 741 is used as a voltage comparator to switch on the DC fan. Its INV input (pin2) gets an adjustable voltage through VR while its non-INV (pin3) input gets voltage through a potential divider comprising R1 and the Thermistor. Thus, the voltage at pin3 
depends on the conductivity of the Thermistor.

**_Circuit Working Video_** 
![ezgif com-video-to-gif](https://github.com/Drupad-DeV/Temprature-Controlled-DC-Fan-Using-Lm741/assets/100958162/ea7ffedc-8e36-4878-8b2d-49c501eaadc1)



