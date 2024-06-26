# PythonOCC Nodes for NodeCAD
Pythonocc nodes package for Ryven.

Here a way to work on Pythonocc with a node editor, Ryven in that case.
To get it functional you will have to execute Ryven in an environment where pythonocc is installed.

### Usage

First you need to install NodeCAD: https://github.com/HakanSeven12/NodeCAD

When installed, create a directory ~/.ryven/ in your user home with the following structure:
```
~/.ryven
├── nodes
    ├── PythonOCC
        ├── nodes.py
        └── gui.py
```

### Examples


![example1](https://github.com/HakanSeven12/NodeCAD/blob/main/screenshots/example1.png)

![example2](https://github.com/HakanSeven12/NodeCAD/blob/main/screenshots/example2.png)


It's just a beginning to explore the possibilities given by matching the two, I've just coded simple functions to see how it works and how it should be to perform complex operations.

### Contribute !

The nodes are of course open for contribution, as there are thousands of functions in OpenCascade and thousands of ways to develop properly the nodes!

The functions currently implemented are:

`Gp_nodes = Pnt_Node, DeconstructPnt_Node, PointZero_Node,Dir_Node, Vec_Node, DX_Node, DY_Node, DZ_Node,Ax2_Node, Pln_Node, Trsf_Node, Move2pts_Node, MidPoint_Node,`

`BRepBuilderAPI_nodes = TwoPtsEdge_Node, Wire_Node, WireFillet2d_Node, DiscretizeWire_Node, Get_dir_from_edge_Node`

`BRepOffsetAPI_nodes = Pipe_Node,`

`BRepPrimAPI_nodes = Box_Node, Sphere_Node, Cylinder_Node,`

`BRepAlgoAPI_nodes = Fuse_Node, Common_Node, Cut_Node,`

`BRepFilletAPI_nodes = fillet_Node,`

`GeomAPI_nodes = PointsSurface_Node,`

`TopExplorer_nodes = TopExplorer_Node,`

`Display_nodes =  display_Node, Color_Node,`

`Tools_nodes = List_Node, ListLength_Node, FlattenList_Node, ListItem_Node, RepeatData_Node, Serie_Node, ShiftList_Node,`

`DataExchange_nodes = ExportStep_Node, ImportStep_Node, ExportStl_Node, ImportStl_Node, ExportGcode_Node`

Each "nodes" family is a class with a color attributed. Node names are correspond to the functions from Pythonocc.

To add a function from Pythonocc you have to generate a code as shown in `add_function_box_example.py`.
