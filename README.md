# WindSite_AI

Challenge - 
Design an AI-powered tool that analyses multiple data sources to recommend or allow a search for good potential sites for future windfarm development. The solution should:​
Evaluate land suitability based on environmental, regulatory, and operational criteria. (site selection)​
Surface insights about expected wind resource and power output. (site modelling)​
 ​
Feature Teams Could Build​
Interactive Map Dashboard: Visualise candidate sites, overlaying key data layers (wind speed, residential properties, environmental constraints).​
Site Scoring Engine: Rank plots based on configurable criteria (wind resource, proximity to other wind farms, proximity to residential properties etc).​
Scenario Modelling: Allow users to adjust wind turbine size and compute cost and potential wind farm yield.​
Automated Reporting: Generate summary reports for shortlisted sites, including rationale and yield and costs assessments.

Data - 
The dataset will include files (shapefile, .csv, GeoTIFF) for the following constraints. “Setback” stipulates how far the development must be from the geographic feature.​
​
In addition to these constraints, please consider the following information when modelling the cost and yield of a potential site:​
​
Wind speed @100m (given as GeoTIFF)​
Formula for potential energy yield of wind farm: Energy [KWh] = 0.6 * ½ ρ * (3.14 * 0.25 * D^2) * v³ * 8760 *no.turbines*(1/1000_000)​
Where ρ is air density (assume 1.2 kg/m^3), D is the rotor diameter of the turbine, v is wind speed, 8760 is hours in a year, no.turbines is the number of turbines that fit into the site, (1/1000)000) Watts in MegaWatt.​
Spacing of wind turbines should be at least 5 rotor diameters apart​
Cost of different sizes of wind turbine:​
160m rotor diameter / £2.5million per turbine​
130m rotor diameter / £1.6million per turbine​
100m rotor diameter / £1million per turbine​
​
​
Constraint​
Setback​
Residential properties​
1km​
Water Bodies​
50m​
Public Highway​
Tip height + 10%​
Railway​
Tip height + 10%​
Other renewable energy developments within 5km​
0m​
Ancient Woodland​
0m​
Country Parks​
0m​
National Gas Transmission Pipeline​
1.5x Hub Height​
ECOLOGICAL DESIGNATIONS​
0m​
SSSI - Site of Special Scientific Interest​
0m​
NNR - National Nature Reserve​
0m​
LANDSCAPE / AMENITY DESIGNATIONS​
0m​
NSA - National Scenic Area​
0m​
National Parks​
0m​
HERITAGE DESIGNATIONS​
0m​
WHS - World Heritage Site​
0m​
Conservation Areas​
0m​

Tips - 
Guide:​
What land is available to develop on after considering constraints?​
How many turbines could I fit on these areas? (will depend on the size of turbine)​
How does this affect cost and energy yield of the potential site?​
