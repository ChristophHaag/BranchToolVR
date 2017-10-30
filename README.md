# BranchToolVR

A tool designed to map vascular systems present in medical images in virtual reality. The previous non-vr iteration of the tool can be found here: https://github.com/microdr/Branch-Tool

## TODO list:
- [ ] continue work on vein tracing using controller position
- [ ] transparent object depth sorting - ?
- [ ] auto detect sensible windowing values - ?
- [ ] data set testing
- [ ] clamp point cloud selector box within bounds - done
- [ ] fix bounding sphere generation and collision testing
- [ ] add isovalue coloring to static mesh
- [ ] refactor shaders
- [ ] combine proj and view matrices on cpu
- [ ] refactor screen ui
- [ ] sort points by isovalue for faster surface lookup
- [ ] declare const where possible in class functions
- [ ] add object manager class
- [ ] refactor code from other sources
- [ ] re-enable shadows - not right now
- [ ] refactor shaders to class objects
- [ ] add virtual draw function to inherited class
- [ ] point cloud culling - not right now
- [ ] refactor class/struct destructors
	- [ ] delete opengl data in renderer destructor
- [ ] refactor class privelages
- [ ] identify performance bottlenecks
- [ ] include all .psd and .blend files in repo
- [ ] add visual feedback to actions
- [ ] repository features
- [ ] assign object type ids automatically
- [ ] add selector cube model (remove transparency)
	- [ ] <sup>add compile instructions</sup>
	- [ ] <sup>create libraries zip in download section</sup>
	- [ ] <sup>uml documentation</sup>
- [ ] triangulate vein structures
- [ ] export triangulation (traced veins to blender)
- [ ] file dialog for DicomSet selection
- [ ] separate classes to follow single responsibility rule
- [x] DICOM image in 2D window renders as black when HMD is connected
- [x] Change tracing from Grip buttons to trigger button toggles
- [x] Add spoof input key for the app menu button
- [x] Add spoof input key for the touchpad which initializes a new curve
- [ ] Zooming/Scaling the voxels
- [x] Remap the new curve button to the touchpad
- [x] Remap the create sphere action to the trigger
- [ ] Collision between voxels and the ray from controller to generate spheres
	- [ ] Instead make the controller pointer shorter and use the tip to generate spheres, no collision detection necessary
- [x] Make the branch point marking spheres smaller
- [ ] Export curve coefficients and points
- [ ] Generate isosurface of tumor from the point cloud and export

## Libraries used:
* OpenGL
* OpenVR
* GLFW
* GLM
* imebra
* tinyobjloader
