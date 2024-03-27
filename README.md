![header](https://github.com/JeremSparte/BHToolset/assets/123566406/12acba29-f4ea-4faa-aa0b-88e106ee421a)

## Description

This is an open-source Houdini project to generate climbing holds geometry to print in 3D. Many ready-to-print STL files are availables to download.  
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

![stillbanana](https://github.com/JeremSparte/BHToolset/assets/123566406/bab0f1e3-8ad9-4b09-8256-2f925854b015)

### BH Mold

It is a straight forward tool, it transforms your climbing hold into a mold, ready to fill with whatever you want.

![stillbananamold](https://github.com/JeremSparte/BHToolset/assets/123566406/4850e644-5f57-4bd7-b4e3-a4f9382e983c)

### BH Structure viewer

This is a quick visualizer to highlight thin parts of your geometry, can be bad to see too much blue !

![stillbananastruct](https://github.com/JeremSparte/BHToolset/assets/123566406/840e0336-839e-4b1d-8b50-725a88a05419)

## Library

I generated [144 STL files](/samples) as a sample.  
There are [4 examples of images](/assets/Shape) for the FromPic node. 

![Render_ALL](https://github.com/JeremSparte/BHToolset/assets/123566406/0cf5bdaa-87e1-47c1-803f-646bf9c90632)

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

## License

[MIT](https://choosealicense.com/licenses/mit/)
