# ETABSPlugins

## Latest Version v1.0.0 

## Invest in Arup Projects
[26240 Useful Plugins for Structural Analysis Softwares](https://invest.arup.com/?layout=projsheet&projid=26240&tab=projsheetdetailstabpage0)

[29152 Useful Plugins for Structural Analysis Softwares Part 2](https://invest.arup.com/?layout=projsheet&projid=29152&tab=projsheetcommentstabpage0)

## License 

Compatible with ETABS 18 and newer versions

## Users - Download release

To use the plugins you can download the latest release from the [releases section](https://gitlab.arup.com/Gokberk.Isik/etabsplugins/-/releases).

## Bug reporting

Please report bug by [opening a new issues](https://gitlab.arup.com/Gokberk.Isik/etabsplugins/-/issues) and use the provided **bug report** templates

## New features

Please submit feature requests by [opening a new issues](https://gitlab.arup.com/Gokberk.Isik/etabsplugins/-/issues) and use the provided **new features** template

## Requirements

In order to use these plugins you will need to add them by using "Add/Show Plugins" option under "Tools" main menu. Status should be "OK".

![Add_show_plugins](./Docs/Add_show_plugins.png)

![Browse_Etabs_Main_dll](./Docs/Browse_Etabs_Main_dll.png)

## Main Interface

![Main_interface](./Docs/Main_interface.png)

## Pre-processing Works

### Load Combination Generation

All load combinations are in accordance with short-period design spectral response acceleration parameter (Sds) and Overstrength Factor (D) depending on whether building has a basement or not.
For now, compatible with TEC2018 only. 
Combination File: 
2-COMBINATIONS FOR TEC 2018.docx 
Location: 
\\global\europe\istanbul\DISCIPLINES_AREA\YAPI GRUBU\15 DIGITAL STRUCTURE GROUP\NEW SIESMIC CODE\SPREADSHEETS\ 

###	Shear Wall Pier Assignment

In order to obtain and evaluate the internal forces of shear walls which are modelled with shell elements in the structural model, it is necessary to assign a pier section (pier names). Instead of assigning pier names into shear walls individually for each floor, this plugin can assign them all by simply clicking a button with defined prefixes. Starting from zero, names are given according to the positions of the shear walls segments in X and Y axis.
Also, it is possible to save pier names or reload preassigned pier names from a csv file.

## Post-processing Works

###	Pier Shear Check 

This plugin extracts all the shear wall properties and pier forces. Then it calculates required shear capacities according to the specified code. 

###	Column Axial Capacity Check

With the help of this plugin, all user-defined material properties and forces can be extracted and detailed column axial capacity checks can be performed according to the specified code. Also, it is possible to define design ratio limits and possible to assign the columns exceeding these limits to the desired groups if AssignGroups option is ticked.

###	Beam Axial Load Check

This plugin can extract all the beam properties, forces and will perform beam axial capacity checks according to the specified code. Also, it is possible to define design ratio limits and possible to assign the beams exceeding these limits to the desired groups if AssignGroups option is ticked.

###	Beam Shear Check and Reinforcing

This plugin can extract all the beam properties, forces and calculate required draft shear reinforcement areas according to specified code. Also, it is possible to define design ratio limits.

### Response Spectrum Comparison
With this plugin, it is possible to compare different response spectrum created by ETABS with simple selections.

## LS-Dyna Extraction Tools 

###	Model Geometry Extract for LS-Dyna
This plugin exports of all node, frame, shell geometry properties and their connectivity to CSV files in accordance with LS-dyna part definitions. In this way, LS-Dyna models are created by the help of auto mesh options of ETABS program.

### Concrete Beam Property Extract for creation of Park_Ang_Beam(MAT206)
Creation of Park ang Beam material properties is a long process that had to be prepared individually for each section type and reinforcement properties in accordance with Moment-Rotation curves. This plugin creates the necessary CSV files from ETABS to automatize this process.


