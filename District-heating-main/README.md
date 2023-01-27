# District-heating

Data can be loaded via https://mapeditor.hesi.energy/editor# (need an account) 
1) draw an area and rightclick and 'press request BAG building' to load BAG data
2) Not all buildings are loaded, these can be handdrawn by selecting building, drawing polygons and filling in extra building information.
	- Make sure you add an BuildingUnit to the buildings Asset with the right info in it
3) Add a HeatNetwork, HeatingDemand and ElectricityDemand somewhere
	- The HeatNetwork must be placed at the point where the central pipe will be split off into the individual pipes
4) Add a heater (like BiomassHeater) for the HeatNetwork and place it on its wanted location. The same goes for HeatStorage
5) Save and add file to folder where District-heating is. Make sure the file name corresponds to the one found in f_startupESDLimporter