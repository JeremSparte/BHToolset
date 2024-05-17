![header](https://github.com/JeremSparte/BHToolset/assets/123566406/12acba29-f4ea-4faa-aa0b-88e106ee421a)

## Description

This is an open-source Houdini project to generate 3D printable climbing holds.  
Ready-to-print STL files are available to [download for free](#library).  
  
The main screw is a [CHC 10x50](https://euroholds.com/en/bolts/44-chc-10x50-8435561602363.html) and the other optional small ones are [PZ 4x40](https://www.demos-trade.eu/strongfix-screw-pz-4x40-with-countersunk-head-white-zinc-pz2/) wood screws.

## Installation

Use [Houdini](https://www.sidefx.com/products/houdini/) 19.5/older.

## Usage

### BH FromPic

This node is a All-in-one hold generator from a picture. Each color channel represent a source for the generator to work properly.  
You can edit the .psd file in the repo, everything is already inside. Use Photoshop or [Photopea](https://www.google.com) (free).  
Red is for a scale, it represent 1 centimeter.  
Green is for the shape of the hold.  
Blue is for the screws, the bigger is the main screw and the others smaller ones are optionals.

https://github.com/JeremSparte/BHToolset/assets/123566406/967cd841-3988-4733-985c-31aaf3e468ac

### BH Shaper

This node is a simple geometry generator, it subtracts another sphere on top for the finger grip ('imprint parameter').  
This node is useful to generator all sort of holds by its noise variations.  
Combine with the BH_Holder node to obtain a ready to print asset.

https://github.com/JeremSparte/BHToolset/assets/123566406/e5006ef7-98a9-424b-9d7a-f82b64c28e77

### BH Holder

This is the core tool, it transforms any 3d geometry in a hold. It split the geometry apart on the Z axis.  
You can have control on the screws positions. To preview them merge the two outputs.  
It combines well with photogrammetry to transform day-to-day objects in boulder holds.

![BananaHold](https://github.com/JeremSparte/BHToolset/assets/123566406/9f0f2716-bddb-4bdc-897e-262b4f20de45)

### BH Mold

It is a straight forward tool, it transforms your climbing hold into a mold, ready to fill with whatever you want.

![BananaMold](https://github.com/JeremSparte/BHToolset/assets/123566406/72dc683f-f81c-48d9-91cb-fb4c1ae9c46f)

### BH Hollow

Allows you to make a hollow version of your hold to fill it later with the material of your choice.

![BananaHollow](https://github.com/JeremSparte/BHToolset/assets/123566406/a1a3777a-fb83-47aa-9a6c-34bea8743997)

### BH Structure viewer

This is a quick visualizer to highlight thin parts of your geometry, can be bad to see too much blue !

![BananaStructure](https://github.com/JeremSparte/BHToolset/assets/123566406/f4977bf7-ccd7-4e00-bd3c-7a39825dbba0)

# Library

[Download here !](https://www.printables.com/@JeremyLAFAYE_2080610)  

![Render_ALL](https://github.com/JeremSparte/BHToolset/assets/123566406/c5f0ce40-e5f4-4d90-b2e4-b6e08e77b858)
![RS_Collection](https://github.com/JeremSparte/BHToolset/assets/123566406/a2fb3eca-4365-4542-aca5-78a1d811679c)
![Library](https://github.com/JeremSparte/BHToolset/assets/123566406/9ca6f68e-fb67-4a3e-a38d-46cb724e4efd)

All of these sample are fully generated from the tools and can be downloaded for free on [Thingiverse](https://www.thingiverse.com/sardou3d/designs), [Printables](https://www.printables.com/@JeremyLAFAYE_2080610) and [Cults3D](https://cults3d.com/en/users/SarDou3D).

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
