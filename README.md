
# District Heating

District Heating is a tool written by Mels Habold for his internship at ZEnMo. This tool creates a digital twin of a neighbourhood (in this case Apeldoorn Noord or in Rotterdam) and allows the user to play around with some buttons which change the energy dependencies of this neighbourhood. This tool utilizes code from a lot of different other tools created by ZEnMo, but mostly it looks at the impact of having a heating network in your neighbourhood as opposed to having local boilers. 

### Installation

This tool is based in the Agent Based Language called Anylogic, which combines a visual mode of programming with javascript. Installment can be done by installing Anylogic via their site. Warning, a student licence is needed.

Data can be loaded via https://mapeditor.hesi.energy/editor# (need an account)

    draw an area and rightclick and 'press request BAG building' to load BAG data
    Not all buildings are loaded, these can be handdrawn by selecting building, drawing polygons and filling in extra building information.
        Make sure you add an BuildingUnit to the buildings Asset with the right info in it
    Add a HeatNetwork, HeatingDemand and ElectricityDemand somewhere
        The HeatNetwork must be placed at the point where the central pipe will be split off into the individual pipes
    Add a heater (like BiomassHeater) for the HeatNetwork and place it on its wanted location. The same goes for HeatStorage
    Save and add file to folder where District-heating is. Make sure the file name corresponds to the one found in f_startupESDLimporter


### Features

This tool looks at the costs (both investing and operational) and environmental impacts. Additionally, the tool also has modelled the energy needs of industries, whereas normally it only looks at households. It is also possible to download objects from ESDL (specifically the Map editor). The tool consists of an underlying model and a graphical interface layerd above it. 

More information about the underlying model can be found in the internship report.
