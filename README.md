Filter Explorer
===============

Filter Explorer application demonstrates some of the image editing capabilities
and performance of the Nokia Imaging SDK by allowing you to apply a number of
filter layers to existing or newly captured photos.

The example has been developed with Silverlight for Windows Phone devices
and tested to work on Nokia Lumia devices with Windows Phone 8.

This example application is hosted in GitHub:
https://github.com/nokia-developer/filter-explorer

For more information on implementation, visit Nokia Lumia
Developer's Library:
http://developer.nokia.com/Resources/Library/Lumia/#!nokia-imaging-sdk/sample-projects/filter-explorer.html


1. Usage
-------------------------------------------------------------------------------

This is a simple build-and-run solution. See section 5 for instructions on how
to run the application on your Windows Phone 8 device.


2. Prerequisites
-------------------------------------------------------------------------------

* C# basics
* Windows 8
* Development environment Microsoft Visual Studio Express for Windows Phone 2012


3. Project structure and implementation
-------------------------------------------------------------------------------

3.1 Folders
-----------

* The root folder contains the project file, the license information and this
  file (release_notes.txt).
* `ImageProcessingApp`: Root folder for the implementation files.  
 * `Assets`: Graphic assets like icons and tiles.
 * `Controls`: Custom UI controls.
 * `Converters`: Utilities to convert various data types in XAML.
 * `Helpers`: Rendering, tombstorning, etc. helpers.
 * `Models`: Application model.
 * `Pages`: XAML pages.
 * `Properties`: Application property files.
 * `Resources`: Application resources.


3.2 Important files and classes
-------------------------------

| File | Description |
| ---- | ----------- |
| `Helpers/StreamRenderingHelper.cs` | Helper utilities for fast photo stream rendering. |
| `Models/FilterModel.cs` | Different individual filters. |
| `Models/PhotoModel.cs` | Main model class including photo data, editing session and rendering functions. |
| `Pages/FilterPage.xaml(.cs)` | Filter selection page. |
| `Pages/PhotoPage.xaml(.cs)` | Main selected photo display/editing page. |
| `Pages/StreamPage.cs` | Startup page, displays Camera Roll photos rendered with randomly applied filters. |


3.3 Used Nokia Image Editing APIs
---------------------------------

* Nokia.Graphics
* Nokia.Graphics.Imaging
* Nokia.Graphics.Utilities


4. Compatibility
-------------------------------------------------------------------------------

* Windows Phone 8

Tested to work on Nokia Lumia 520, Nokia Lumia 620, Nokia Lumia 820 and Nokia
Lumia 920. Developed with Microsoft Visual Studio Express for Windows Phone 2012.


4.1 Required Capabilities
-------------------------

* `ID_CAP_MEDIALIB_PHOTO`


4.2 Known Issues
----------------

None.


5. Building, installing, and running the application
-------------------------------------------------------------------------------

5.1 Preparations
----------------

Make sure you have the following installed:
 * Windows 8
 * Windows Phone SDK 8.0

5.2 Using the WINDOWS PHONE 8 SDK
---------------------------------

1. Open the SLN file:
   File > Open Project, select the file ImageProcessingApp.sln
2. Select the target 'Device' and 'ARM'.
3. Press F5 to build the project and run it on the device.

5.3 Deploying to Windows Phone 8
--------------------------------

Please see official documentation for deploying and testing applications on
Windows Phone devices:
http://msdn.microsoft.com/en-us/library/gg588378%28v=vs.92%29.aspx


6. License
-------------------------------------------------------------------------------

See the license text file delivered with this project. The license file is also
available online at
https://github.com/nokia-developer/filter-explorer/blob/master/Licence.txt


7. Version history
-------------------------------------------------------------------------------

* 1.1.0.0 Updated looks, new green theme.
* 1.0.0.0 First public release.
