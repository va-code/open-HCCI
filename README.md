# open-HCCI
An open source HCCI Engine design as easy to retrofit to existing engines as a turbo

The design consists of:
1. Adding a high pressure compressor to the engine(probably low volume)(higher pressure than autoignition temp of fuel)
2. Removing the spark plugs and replacing them with special high pressure valve assemblies
3. Porting the high pressure compressor output to the valve assemblies
4. Electronically controlling the valves to input a set volume of high pressure air to the combustion chamber after TDC.
5. The high pressure air then autoignites the chamber.
6. the gasses exhaust and the valve assembly resets to the predetonation state ready for next cycle.


Issues with the design:
Since the combustion is not caused by pressure increase but the associated temperature increase there are probably problems with the thought in the design:
1. the added gasses would be expanding and lossing pressure thus making them cool down further possibly negating the objective. It still might work if pressure spikes fast enough that the chamber gasses dont mix much with the compressed air shot.
2. Testing will be needed to check if a feasible result is attainable.
3. Some efficiency losses will come from the compressed air cooling down before getting routed to the cylinders

Fixes:
1. Compress exhaust gasses instead of ambient to get higher temperature and possible pressure gasses before the compressor to save efficiency and reliability of the system
2. Store the compressed air surrounded by exhaust manifold and insulation to maintain temp.
