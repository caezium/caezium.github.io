# Analogue to Digital Converter (**ADC**)

A computer cannot make sense of physical quantities such as pH, celsius, etc.

To convert physical quantities to a digital format, an ADC needs to be used, it converts physical values/analogue data into digital data that is readable by the computer.



how to answer: 
1. Actuator
2. Sensors
3. ADC
4. Microprocessor
5. Preset value
6. DAC?
7. Signal
8. Continuous?




Continuous loop, preset value, sensor detects -> ADC -> microprocessor computes data and calculate what to do -> sends to output and performs the action



# Common Sensors
## Temperature
measures temp of surrounding env by sending signals

control a central heating system
monitor/control chemical processes
greenhouse temp


## Moisture
measures water levels, such as in soil

control/monitor moisture levels in soil in a greenhouse
in food processing factories to prevent moisture levels from spoiling food


## Humidity
measures the amount of water vapor in , ex. a sample of air

monitor humidity levels in a factory so that ex. it doesn't corrode parts/short circuit
monitor/control in greenhouse

## Light
utilizes photoelectric cells that generate an electric current output based based on the brightness of the light

switching street lights on or off depending on light levels
car headlights auto


## Infrared
detects infrared radiation emitted by objects to determine their presence of proximity

turn on windscreen wipers auto
security alarm system

## Pressure
measures the force exerted on its surface

weighing of lorries at a weighing station
gas pressures in plants/factories


## Sound
detects sound waves and converts them into electrical signals

security system
liquids dripping at faulty pipe joint

## Gas
detects presence and concentration of gases in the env

monitor oxygen and carbon dioxide levels in a greenhouse

## PH
acidity or alkalinity of a solution

monitor/control acidity in greenhouse


## Magnetic field 
strength and direction of the magnetic field


## Accelerometer
measures acceleration forces, enabling orientation and movement detection

cars rapid deceleration for airbags
phone for games


## Proximity
how close an object is

phone turns dark when near ear


## Flow
rate of fluid flow

respiratory devices and inhalers in hospitals
in pipes

## Level
level or amount of substance in a container or reservoir

petrol tank in a car
leak detection in refrigerant





![[02_areas/COMP SCIENCE/3/attachments/c3940d745b45604ac59a20f813791ad1_MD5.jpeg]]
An infrared sensor detects the infrared radiation emitted by objects to determine their presence of proximity by the finish line to check if a competitor crosses the finish line. The signal is sent to the microprocessor using ADC, converting analogue data into digital data that is able to be interpreted by the microprocessor. The microprocessor gets the preset value of what proximity/line the runner has to be in order to count it as crossing the finish line, and compares the value with the data sent to it. If crossed the competitor is marked as finished, logging and incrementing the count of how many competitors finished the race. This repeats in a continuous loop.


Sensor sends signal to microprocessor
signal is analogue and is converted to digital using ADC
compared to stored value/check for signal
if data matches/in range counter is incremented by 1
continuous process