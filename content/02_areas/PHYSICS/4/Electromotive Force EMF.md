>[!def] EMF
>The work done per unit charge by a source in driving current around a complete circuit. It represents the total energy converted from another form (chemical, mechanical, etc.) to electrical energy per unit charge.

## Basic Concepts

### Definition and Units
- Measured in volts (V)
- Symbol: ε (epsilon)
- Energy per unit charge
- Driving force for current

### Sources of EMF
1. **Chemical**
   - Batteries
   - Fuel cells
   - Chemical reactions

2. **Mechanical**
   - Generators
   - Dynamos
   - Motion in magnetic field

3. **Light**
   - Solar cells
   - Photoelectric devices
   - Light energy conversion

4. **Thermal**
   - Thermocouples
   - Temperature difference
   - Seebeck effect

## EMF vs Terminal Potential Difference

### Internal Resistance
- Present in all real sources
- Symbol: r
- Causes voltage drop
- Reduces terminal voltage

### Terminal Voltage
1. **No Current (Open Circuit)**
   - Terminal voltage = EMF
   - Maximum potential difference
   - No internal voltage drop

2. **With Current Flow**
   - Terminal voltage < EMF
   - V = ε - Ir
   - Voltage drop across internal resistance

## Circuit Analysis

### Lost Volts
- Voltage drop in source
- Due to internal resistance
- Ir = Lost volts
- Reduces circuit efficiency

### Circuit Equations
1. **Complete Circuit**
   - ε = IR + Ir
   - EMF = External voltage + Lost volts
   - I = ε/(R + r)

2. **Power Relationships**
   - Total power = εI
   - Useful power = VI
   - Lost power = I²r

## Practical Applications

### Battery Characteristics
1. **Fresh Battery**
   - Maximum EMF
   - Low internal resistance
   - High efficiency

2. **Aging Battery**
   - Decreasing EMF
   - Increasing internal resistance
   - Reduced efficiency

### Power Supplies
1. **Ideal Sources**
   - Constant EMF
   - Zero internal resistance
   - Theoretical concept

2. **Real Sources**
   - Variable EMF
   - Significant internal resistance
   - Temperature effects

## Measurement Techniques

### EMF Measurement
1. **High-Resistance Voltmeter**
   - Minimal current draw
   - Close to true EMF
   - Open circuit measurement

2. **Potentiometer Method**
   - Null method
   - Accurate measurement
   - No current drawn


>[!note] Key Understanding
>EMF is the driving force that maintains current flow in a circuit, converting non-electrical energy into electrical energy. The actual voltage available for use (terminal voltage) is always less than the EMF due to internal resistance.

>[!example] Practical Example
>For a 12V battery with internal resistance 0.5Ω, supplying 2A:
>- Lost volts = 2A × 0.5Ω = 1V
>- Terminal voltage = 12V - 1V = 11V
>- Power lost internally = (2A)² × 0.5Ω = 2W
