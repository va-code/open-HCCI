# open-HCCI
The goal of this project is to design and test an open source HCCI Engine as
easy to retrofit or add to existing designs as a turbo.

# Intro
HCCI (Homogeneous Charge Compression Ignition) engines work by compressing a
well mixed fuel and gas mixture until they autoignite.
https://en.wikipedia.org/wiki/Homogeneous_charge_compression_ignition
This can be difficult to achieve due to a typically fixed compression ratio
of pistons and certain parts of the engine retaining heat and causing
ignition before TDC. The benefits of an HCCI engines are primarily the extremely lean fuel ratios(more fuel efficient), and lowed emisions.

In this concept the final amount of compression to reach autoignition is
supplied after TDC by a valve assembly that spikes the pressure above
autoignition rapidly. The autoignition further increases the pressure above
the regulated input. Because of this, in a simple design, a one way check
valve can be used to stop the combustion gases from going back to the
solenoid valve and tank. After ignition the solenoid valve connecting to the
supply air is closed and the piston is allowed to go through powerstroke and
exhaust as normal. The valve solenoid is only opened again breifly after the
next power strokes TDC. 

# The Design:
1. Adding a high pressure compressor to the engine(probably low volume)(higher pressure than autoignition temp of fuel)
2. Removing the spark plugs and replacing them with special high pressure valve assemblies
3. Porting the high pressure compressor output to the valve assemblies
4. Electronically controlling the valves to input a set or variable volume of high pressure air to the combustion chamber after TDC.
5. The high pressure air then autoignites the chamber.
6. the gasses exhaust and the valve assembly resets to the predetonation state ready for next cycle.


# Issues with the design:
Since the combustion is not caused by pressure increase but the associated temperature increase there are probably problems with the thought in the design:
1. the added gasses would be expanding and lossing pressure thus making them cool down further possibly negating the objective. It still might work if pressure spikes fast enough that the chamber gasses dont mix much with the compressed air shot.
2. Testing will be needed to check if a feasible result is attainable.
3. Some efficiency losses will come from the compressed air cooling down before getting routed to the cylinders.
4. No Simulation or math has been done on whether the mockup stl files can withstand the applied forces for specific materials.

# Fixes?:
1. Compress exhaust gasses instead of ambient to get higher temperature and possible pressure gasses before the compressor to save efficiency and reliability of the system
2. Store the compressed air surrounded by exhaust manifold and insulation to maintain temp.
