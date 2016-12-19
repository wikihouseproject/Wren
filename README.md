# WikiHouse Wren

The language and rules for the Wikihouse structural system for 1-3 storey buildings, initially developed in the UK for European contexts.

![alt tag](https://github.com/wikihouseproject/Wren/blob/master/Images/Wren_overview.jpg)

## Wren Hardware

Wren components are CNC manufuctured using structural-grade timber panel materials (typically, plywood) and can be rapidly assembled to produce a structural chassis, onto which other components such as cladding, windows, doors can be fitted.

Wren is in development. For full documentation on how Wren works and how you can contribute to its development, visit the [Wren wiki](https://github.com/wikihouseproject/Wren/wiki)

## Wren Parametrics

This version of the Wren structural language has been developed in Grasshopper, the parametric scripting plugin for Rhino 3D. This computational design platform is widely used in the design and construction industries, and is ideally suited to digital manufacturing.

Other formats of the Wren system are currently being developed, but currently this version in Grasshopper XML format represents the latest thinking and workflow for the structural technology.

It should be taken as a Work in Progress and follows ‘a build something that works first’ approach. There are still several known areas where efficiency can be improved. There are also many ways the script can be extended to make use of Grasshopper’s expansive suite of tools include new features like structural analysis, nesting, GIS data, and solar/environmental tracking. We gladly welcome contributions from fellow computational designers to fork and develop!


### Licence

The repository Grasshopper file WikiHouse_WREN_(v4.2.3) has been developed by Architecture 00.  

It is licensed under Mozilla Public Licence (MPL) version 2.0. For full legal terms of this licence visit: https://www.mozilla.org/en-US/MPL/2.0/

### Plugins

This script makes use of the excellent developers toolbox of Grasshopper plugins, which makes this all possible. You will need to download and install the latest versions of these plugins from Food4Rhino.com before opening and running this script file.

The plugins used are:

- [Leafcutter](http://www.food4rhino.com/app/leafcutter-google-sheets-grasshopper) - for google sheets integration
- [Elefront](http://www.food4rhino.com/app/elefront) - for automated Grasshopper-to-Rhino flow
- [Human](http://www.food4rhino.com/app/human) - for automated Grasshopper-to-Rhino flow
- [Metahopper](http://www.grasshopper3d.com/group/metahopper) - for batch exports and script analysis

### Known issues / limits

- **D-Joint splitting of the frame** - there is currently a very basic version of the logic but this probably needs to be custom scripted. The basic rules are no section should be larger than the sheet material (nominally 1220 x 2440mm) and D-joints are never closer than two grips to any corner/junction
- **Integration with Google Sheets** - While you can ‘drive’ the Wren script using the parameter sliders, the best way makes use of the Leafcutter plugin, which connects the script with a google spreadsheet for the input and output of project data. This is particularly handy when setting out the window and door sizes and locations.
- **Number of roof points** - Here be bugs, it may not work for multiple roof points and may also break the frame/sheathing geometry. Use with care.
- **Tolerance** - While tolerances can be added to slots in the 3D model, a much better/safer approach is to add tolerance offsets to the final nested cutting files, and keep the 3D geometry at 0mm tolerance.
- **Data structures** - within the component clusters. This can be streamlined even further
- Custom scripts - custom C# / Python scripts can and should be added to replace large sections of the script to improve the flow and speed up processing
- **End-walls (in development)** - The gable end walls use the Wikihouse Weaver system (cassette-based) and still more development needed on an automated workflow here, specifically with how the front and rear facades are divided up around window openings. The parametric script for Weaver is not yet included in this initial release.
- **Notes/comments** -  There’s a definite lack of these in the clusters and subclusters. More detail and comments will be added soon, my apologies! If you have particularly questions get in touch via email or raise an issue here.

## Wren Hardware R&D Contributions

**Architecture 00** (www.architecture00.net)
- [Alastair Parvin](https://twitter.com/AlastairParvin)
- [David Saxby](https://twitter.com/davidsx00)
- [Ryan McLoughlin](https://twitter.com/ryanjamesmac)
- [Clayton Prest](https://twitter.com/ClaytonPrest) 
- [Nick Ierodiaconou](https://twitter.com/nick_diaconou) 
- [Joni Steiner](https://twitter.com/jonisteiner)

**Momentum Engineering** (www.momentumengineering.com)
- Ben Whitfield
- Steve Fisher
- Rosie Stevenson

**Space Craft Systems** (www.spacecraft.co.nz)
- [Danny Squires](https://twitter.com/ecoarknz)
- [Martin Luff](https://twitter.com/martinluff)

**Arup Associates** (www.arup.com)
- Nina Tabink
- Adrian Campbell


**Individual Contributors**
- [Alex Whitcroft](https://twitter.com/AlexWhitcroft)
- Justyna Swat
- Nico Maes
- Akiko Kobayashi

**ULB Bruxelles**
- Structural engineering student group

## Wren Parametric Contributions

**Architecture 00** (www.architecture00.net)
- [Clayton Prest](https://twitter.com/ClaytonPrest) 

**Architype Architects**
- Agneesh Brahmbhatt

If you believe you are missing from either of these lists of historical contributions, please contact us or fork this document to amend.


# Terms of use

By downloading these files or information you agree to the following terms and conditions.

Information is shared without any kind of warranty or guarantee
All Information is provided ‘as is’. No representations or warranties express or implied are made regarding the Wikihouse Info, its accuracy, completeness, functionality or fitness for a particular use in a particular location.  

You are solely responsible for the use of the information
By using this information you assume full responsibility for any loss resulting from use or inability to use the Wikihouse Info, and forever releases WikiHouse Foundation or other WikiHouse users from any liability for such loss;  including but not limited to loss of profits, goodwill or assets.

You are responsible for meeting local codes and legislation
Users must satisfy themselves regarding the application of statutory requirements, local building regulations, codes, insurance certification or other requirements or recommendations relevant to the location where and materials with which they plan to build. Where required you should always seek the advice of a relevant qualified professional.

You are responsible for using the information in a safe way
 Users are responsible for ensuring that information they use or cause to be used is used in a way which is safe, and is not likely to cause harm during or after manufacturing, construction, use or disassembly.
