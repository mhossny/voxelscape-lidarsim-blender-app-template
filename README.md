![VOXELSCAPE](https://github.com/mhossny/voxelscape-lidarsim-blender-app-template/blob/main/splash_2x.png)

# VoxelScape LiDAR Simulator
LiDAR Sensor Simulation Blender Application Template

## Requirements
- Blender 2.90
- AnimationNodes add-on 2.1.8 

## Installation
### Animation Nodes
- Navigate to Edit > Preferences > Add-ons
- Click the `Install` button
- Select `animation_nodes.zip` and click `Install Add-on`
- Enable add-on by clicking the check box next to `Node: Animation Nodes`


### VoxelScape Template
- Click on the Blender logo (top-left)
- Click on `Install Application Template...`
- Select `VoxelScape.zip` template and click the `Install Template` button


## VoxelScape in Action
- Navigate to `File > New` and find and click the `VoxelScape` application template
- A simple scene of buildings and a lidar sensor will be loaded. 
- In the right panel, the settings for the lidar sensor are available under `AN > Viewport Inputs`
- For live trials, make sure the `Live/Animation` button is checked to move the sensor and visualise live update. 
- For prerecorded animations, make sure the `Live/Animation` button is un-checked. 


### Blender Stuff
- You can add and edit objects as usual using Blender's functionality. 
- To have the object renderable by the lidar sensors do the following;
	- Set `Pass Index` to non-zero value. This is the object label.
	- Assign the object (or parts of the mesh) to a material. A list of material are included in the template file. 


### Exporting PointClouds
- To export pointcloud, labels, intensity and bounding box files, open a teminal and use the follwing command.

	`$ ./Blender -b ~/Downloads/VoxelScape/blender_file.blend --python-text render -- --export_path ~/tmp/lc/`
	
- For help use `-h`


## Animation Nodes
For more on how animation nodes work, please check the [repo](https://github.com/JacquesLucke/animation_nodes). 

## Change Log
- 2021/09/28: Initial Commit


