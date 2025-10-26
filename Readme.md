# cocoaNEC-ut

This is a – not really serious – fork of **Kok Chen's (W7AY)** excellent antenna simulation program **[cocoaNEC](http://www.w7ay.net/site/Applications/cocoaNEC/)**. There are a few (straightforward) things I missed, and that's why I created this fork using the source code Chen generously made available on his website under the GPL.v Note that W7AY became a silent key in April 2025. https://www.w7ay.net/chen/index.html.

You can download the latest release [here](https://github.com/ulthiel/cocoaNEC-ut/releases/latest). I did not sign the code, so if you get an error like "can't be opened because it is from an unidentified developer", you have to open the application for the first time with a right-click and then click Open (see [Apple info](https://support.apple.com/guide/mac-help/open-a-mac-app-from-an-unidentified-developer-mh40616/mac)).

If you have any questions/comments/suggestions, just drop me an [email](mailto:mail@ulthiel.com).

73,  
Ulrich, DK1UT

## Changes

### Functionality
1. Changed Cmd-O and Cmd-N keyboard shortcuts from spreadsheet to NC models.
1. Added xyz coordinate axis labels in geometry view (Output/Views/Geometry/GeometryView.m).
1. Added keyboard arrow controls for geometry view (Output/Views/Geometry/GeometryView.m, Output/NECOutput.*).
1. Moved Directivity and 0dB= labels in azimuth and elevation plot to better positions (Output/Views/Patterns/AzimuthView.m, Output/Views/Patterns/ElevationView.m).
1. Added degree labels in azimuth and elevation plot (Output/Views/Patterns/PatternView.m).

### Internal
1. Made it compile with XCode 10.
1. Fixed a lot of errors and warnings about [ NSApp delegate ] by replacing this with (ApplicationDelegate*)[ NSApp delegate ].
