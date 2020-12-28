# GenGHG
Generative Design Tool to Reduce Embodied GHG Emissions in High-Rise Residential Buildings.
This work has been developed as part of a M.A.Sc. thesis in Civil Engineering at the University of Toronto.


![GenGHG Banner](https://www.dropbox.com/s/5lsjhh7ih4tbfdg/2020.12.28%20Github%20Banner%202.png?raw=1)

# How to use GenGHG?
Make sure you download and install all dependencies and third-party packages. Also, make sure your computer recognizes the path of the following files for initial testing:

# Required files
## Site Conditions Files
Contain the buildings, landmarks, parks, topography, and water instances in mesh format (.OBJ) that describe the surrounding conditions of the site. The listed .obj files were used for the case study described in the original study. Replace them with your study's information following the same order and categorization. The first four items are used exclusively for visualization purposes, the last two are used for calculations. 
- 20200228_Site-Conditions_Landmarks.obj
- 20200228_Site-Conditions_Parks_1.obj
- 20200228_Site-Conditions_Topo_1.obj
- 20200228_Site-Conditions_Water_1.obj
- 20200312_Massings_SemiDetailed.obj: Contains a simplified mesh for each of the site's surrounding buildings
- 20200405_Site-Conditions_Massings_5.obj: Contains detailed mesh of surrounding buildings for visualization purposes only

## CSV Imports:
- x.csv, y.csv, z.csv: X,Y,Z coordinates for target points for views analysis

- x_mass.csv, y_mass.csv, z_mass.csv: X,Y,Z coordintes for building site footprint 

- lca_factors.csv: Structural and envelope LCA factors for embodied GHG emissions calculation

- material_estimates.csv: Normalized estimates for ammounts of concrete (in cubic meters/volume of building space in cubic meters) and rebar (in metric tons or Mg per Mg of concrete). Normalized per cubic meter of concrete of concrete (Mgcon), and cubic meters of building volume (conm3).

<p align="center">
  <img src="https://www.dropbox.com/s/p9pl0fazjom6a2v/2020.12.28%20GenGHG%20GIF.gif?raw=1">
</p>

# Dependencies
## Dynamo 2.6.0 (dynamobim.org)
### Packages: 
- LunchBox for Dynamo (v2018.7.6)
- Dynamo Text (v2.0.1)
- MeshToolkit (v2.0.1)
- Refinery (v0.62.2)
- spring nodes (v203.1.0)
- Ampersand (v2019.12.31)
- Clockwork for Dynamo 2.x (v2.3.0)
- Topologic (v1.0.0)
### Custom Nodes:
- GenGHG_GeometrySYS_2.dyf

<p align="center">
<img src="https://www.dropbox.com/s/535161oyug4u0zp/GenGHG_thumbnail.png?raw=1" width=50% height=50%>
</p>


