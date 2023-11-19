# Supplement material for paper “Repurposing Coal Power Plants into Thermal Energy Storage for Supporting Zero-carbon Data Centers”



## Coal Power Plants Information 
We consider that the operating coal power plants in the ERCOT system as of 2022, except for those scheduled to be retired by 2025, are eligible for retrofitting. Table I shows the information on 12 eligible coal power plants from global energy monitors [1] and US EIA [2]. 

|Plant|	Plant name|	Capacity (MW)|	Start year|	Combustion technology|	Coal type|	Lat|	Lon|	Heat rate (Btu/kWh)|	Emission factor (kg CO2 /TJ)|
| -- | -- | -- | -- | -- | -- | -- | -- | -- | -- |
|1	| Fayette Power Project|	460|	1988|	subcritical|	lignite|	29.92|	-96.75|	10,878|	101,000|
|2	|J. K. Spruce Station|	566|	1992|	subcritical|	sub-bit|	29.31|	-98.32|	10,878|	96,100|
|3	|J. K. Spruce Station|	878|	2010|	subcritical|	sub-bit|	29.31|	-98.32|	9,572|	96,100|
|4	|Limestone Generating Station|	893|	1985|	subcritical|	lignite|	31.42|	-96.25|	10,878|	101,000|
|5	|Limestone Generating Station|	957|	1986|	subcritical|	lignite|	31.42|	-96.25|	10,878|	101,000|
|6	|Major Oak power station|	174.6|	1990|	subcritical|	lignite/sub-bit|	31.09|	-96.70|	12,618|	98,550|
|7	|Major Oak power station|	174.6|	1991|	subcritical|	lignite/sub-bit|	31.09|	-96.70|	12,618|	98,550|
|8	|Oak Grove Plant|	916.8|	2010|	supercritical|	lignite|	31.18|	-96.49|	9,250|	101,000|
|9	|Oak Grove Plant|	878.6|	2011|	supercritical|	lignite|	31.18|	-96.49|	9,250|	101,000|
|10	|Parish Generating Station|	614.6|	1982|	subcritical/ccs|	sub-bit|	29.48|	-95.63|	17,155|	9,610|
|11	|San Miguel Electric Cooperative|	410|	1982|	subcritical|	lignite|	28.70|	-98.48|	11,748|	101,000|
|12	|Sandy Creek Plant|	1008|	2013|	supercritical|	sub-bit|	31.48|	-96.96|	8,409|	96,100|



## Results from all the scenarios
In total we simulate 12 scenarios including two baseline scenario (1) ERCOT 2030 considering retrofitting without additional DCs (2) ERCOT 2030 without additional DC loads and retrofitting. Results of all scenarios can be found in the GitHub:
https://github.com/yifueve/coal_repurpose/tree/main


|Scenarios of Data center and Energy storage technology |	TES|	LIB|	TES & LIB|
| -- | -- | -- | -- |
|Zero-carbon DC, inflexible|	(3)	|(5)	|(9)|
|Zero-carbon DC, flexible|	(4)	|(6)	|(10) |
|Unconstrained DC, inflexible|	Not applicable|(7)	|(11) |
|Unconstrained DC, flexible|	Not applicable	|(8)	|(12) |


|![ezcv logo](https://raw.githubusercontent.com/Descent098/ezcv/master/.github/logo.png)|
|:--:| 
| *Scenario (3) Zero-carbon DC, inflexible* |


|![ezcv logo](https://raw.githubusercontent.com/Descent098/ezcv/master/.github/logo.png)|
|:--:| 
| *Space* |

|Scenarios |	Result path|
| -- | -- |
|(1)	|../ercot_baseline/Results_retro|
|(2)	|../ercot_baseline/Results_baseline|
|(3)	|../ercot_IF_ZC/Results_TES|
|(4)	|../ercot_F_ZC/Results_TES|
|(5)	|../ercot_IF_ZC/Results_LIB|
|(6)	|../ercot_F_ZC/Results_LIB|
|(7)	|../ercot_IF_UC/Results_LIB|
|(8)	|../ercot_F_UC/Results_LIB|
|(9)	|../ercot_IF_ZC/Results_FULL|
|(10)	|../ercot_F_ZC/Results_FULL|
|(11)	|../ercot_IF_UC/Results_FULL|
|(12)	|../ercot_F_UC/Results_FULL|


## Reference

[1] GlobalEnergyMonitor,“GlobalCoalPlantTracker,”GlobalCoalPlantTracker.Accessed:Feb.28,2023. [Online]. Available: https://globalenergymonitor.org/projects/global-coal-plant-tracker/

[2] US Energy Informa-on Administra-on, “Coal-fired electric power plants.” Accessed: Sep. 10, 2023. [Online]. Available: https://www.eia.gov/coal/data.php#prices

[3] EIA,“CapitalCostandPerformanceCharacteris-cEs-matesforU-lityScaleElectricPowerGenera-ng Technologies.” Accessed: Apr. 21, 2023. [Online]. Available: https://www.eia.gov/analysis/studies/powerplants/capitalcost/pdf/capital_cost_AEO2020.pdf

[4] “GenX.”Accessed:May24,2023.[Online].Available:genxproject.github.io/GenX/dev/
