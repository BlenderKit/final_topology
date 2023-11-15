# Final Topology addon for Blender 3D

Blender 3D addon that introduces subdivision snapping, retopo and modeling tools from the 21st century.

This Blender 3D addon features many tools that were missing and also organizes some simple, but essential tools for polygonal modeling.
Enhanced version adds extra tools for professional CAD and automotive industry modellers.

## Features:
 - **Inverse subdivision snapping**: snaps mesh vertices in edit mode so that if the subdivision modifier is used, the resulting surface is as close as possible to the surface.
   - Live, or 'Simulation' mode of this tool, which works realtime during modeling
   - Neighbours levels, Number of iteration settings
   - Single step operator that can be called with a shortcut with arbitrary number of iterations.
- **Unsubdivide** - takes a mesh that resulted from a subdivision modifier being applied (In blender or in any other application) and recreates the original low-resolution mesh.
    -has settings for number of subdivisions, number of iterations of the algorithm. Higher interation numbers yield precise results.
- **Shape Freeze** - Enables to change topology of Subdivision surface model while keeping the resulting shape as same as possible. (TODO)

## Advanced version features:
- **Constraints** - Edit mode constraints that work together with the subdivision surface snapping. By now snapping to plane. Main difference compared to various shrinwrap modifier tricks is that all constraints get evaluated in a loop together with the subdivision surface snapping, so all conditions get optimized.
- **Loop align to normal plane** - takes a loop and aligns it to a plane that is aligned with it's normals directions. 
- **Loop slide optimize** - balances angles that there are between edges of a loop
- **Flatten selection** - simple flatten to median plane operator (Similar to looptools)

## Download
Final Topology add-on is available in [Full Plan subscription](https://www.blenderkit.com/plans/pricing/) to BlenderKit.

## Support

If you face any bug, please create a report in this repository's issue tracker: https://github.com/BlenderKit/final_topology/issues.
If your bug is related to specific model or project and .blend file is required to debug the problem, please create issue in here and also send the .blend file to admin@blenderkit.com with subject mentioning the issue number and/or title.
