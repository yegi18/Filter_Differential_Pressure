# Filter_Differential_Pressure
Case: Vedanta Aluminium Limited 4*600 MW Captive Power Plant(Thermal)
Phase 1 of the plant has 48 Fabric Bag filter compartments divided into 4 passes with 12 compartments each. Task is to analyze the differential pressure accross the compartments and establish a neural network correlating the pressure with factors such as:

1)Coal Flow(Tonnes per hour)

2)Induced Draft Fan current(A)

3)Gross Generation(MW)

4)SOV Pressure(Stream pressure of water used to clean each compartment after choking)

5)Differential Pressure of compartments in proximity

Raw data initially pre-processes.Limits were set for each of the parameters based on ideal limits. 10 key compartments were identified possessing maximum correlation to the individual pass differential pressure. Pearson correlation matrix plotted for each compartments as against all other 47 compartments to arrive at 2-3 compartments with highest correlation for each key performing compartment.

Custom neutral network with 2 hidden layers was trained. Architecture based on theoretical equation relating differential pressure and volume flow rate. Achieved a mean absolute error<100 pa for DP values ranging from 1000 to 3000 Pa.

