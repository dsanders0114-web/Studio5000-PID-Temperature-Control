# Studio5000-PID-Temperature-Control
Industrial PID temperature control simulation in Studio 5000 using PIDE, autotune, and manual override.


This project demonstrates a simulated temperature control loop using the Studio 5000 PIDE instruction.

Features:
- PIDE closed-loop temperature control
- Auto / Manual mode switching
- Manual output override
- Setpoint ramping
- Output limiting (0–100%)
- Simulated thermal process model
- Autotune implementation
- Before / After response comparison

Project Structure:

Main_LAD
- Start/Stop logic
- Auto/Manual mode control
- Setpoint ramping
- Manual CV handling
- Routine calls

PIDE_FBD
- PIDE controller block
- PV input
- CV output
- Gain tuning

PlantSim_ST
- First order thermal model
- Heater gain simulation
- Time constant response
- Temperature clamping

Signal Flow:

Setpoint → PIDE → Controller Output → Plant Model → PV → PIDE

Autotune Results:

Before tuning:
- Slow rise time
- Oscillation
- Poor settling

After tuning:
- Faster response
- Reduced overshoot
- Stable settling
- Smooth controller output

Files:

PID_Temperature_Loop.L5X — Studio 5000 project export  


Skills Demonstrated:

Studio 5000 Logix Designer  
PIDE instruction configuration  
Closed-loop process control  
PID tuning and autotune  
Function block programming  
Structured text simulation  
Industrial controls architecture
