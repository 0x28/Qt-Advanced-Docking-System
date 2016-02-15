# Advanced Docking System
Manages content widgets more like Visual Studio or similar programs.
I also try to get everything done with basic Qt functionality.
Basic usage of QWidgets an QLayouts and using basic styles as much as possible.

## Tested with - Requirements
**Windows**
- \>= Qt 5.5, VC12 or MinGW
- \>= Qt 4.5.3 VC9 - *not as good...*

**Linux**
- Not yet tested

## Build
Open the `build.pro` with QtCreator and start the build, that's it.

## Notes
- *SectionContent* class may safe a "size-type" property, which defines how the size of the widget should be handled.
	- PerCent: Resize in proportion to other widgets.
	- Fixed: Width or height are fixed (based on orientation).

## TODOs
Sorted by priority
- **[DONE]** Improve FloatingWidget (Remove maximize button, only support close-button which hides the widget)
- **[DONE]** Serialize and Deserialize state/size/positions of dockings
- **[90%]** Make compatible with Qt 4.5 (\*ROFL!\*)
- Save and restore FloatingWidget states
- Drop indicator images should be fully visible over the DropOverlay rectangle
- Pin contents: Pins a content and its title widget to the edge and opens on click/hover as long as it has focus

## Bugs
- **[DONE]** Working with outer-edge-drops sometimes leaves empty splitters
- **[DONE]** Clean up of unused e.g. count()<=1 QSplitters doesn't work well

## Credits
- Drop indicator images from:
	http://www.codeproject.com/Articles/140209/Building-a-Docking-Window-Management-Solution-in-W

## License
Not sure yet... It's in development status anyway.