vA3C Cookbook Read Me
===

### Live Demo

<iframe src="http://va3c.github.io/viewer/cookbook/r1/json-build-export-object.html" width=100% height=500px class='overview' >
There is an `iframe` here. It is not visible when viewed on github.com. To view, please see 'Project Links' below.
</iframe>
_vA3C Cookbook: JSON - Build - Export Object_ / [Full Screen]( http://va3c.github.io/viewer/cookbook/r1/json-build-export-object.html )


## Concept

The files here are to help you get started with, for example, building apps that work with [Open Studio]( https://openstudio.nrel.gov/ ).

All the files here can be downloaded and run locally without any cross-origin security issues.

The goal is to help you develop apps that can help you export data from a heavy-duty design app and make that data available on 
the web or locally for easy viewing and collaboration in your browser - all using the Three.js library.

A useful starting point to observing how Three.js creates data and then exports this data to a JSON file.

Live demo: [JSON Build - Export Geometry]( http://va3c.github.io/viewer/cookbook/r1/json-build-export-geometry.html )  
Source code: [JSON Build - Export Geometry](  https://github.com/va3c/viewer/tree/gh-pages/cookbook/r1/json-build-export-geometry.html )

This file creates a Three.js mesh that represents a 50 m by 30 m by 12 stories at 3 M each.

The mesh is rendered in wireframe mode so that you can see all the triangle faces that are generated.

You can zoom, pan and rotate the model using your pointing device.

There is a single command: 'Export geometry', Clicking the button brings up the 'File Save" dialog 
and allows you to export the data to an ASCII JSON file. A default file name is provided, but you can use any name you wish.

Once the file is exported, you may open the file with any text editor and observe how Three.js structures the geometry.
The script exports geometry only. Materials and other scene data is ignored. 

Since the data is just a box, Three.js exports  just the command to create a box and not all the vertices and faces.

Most variables are globals so you can easily inspect their data at any time. 
Most aspects are hard-wired - just because the script is designed to be as simple as possible so as to provide a quick glimpse into structure of the data.

Now that the data has been exported, let's see if you can import the data and view it in 3D.

Live demo: [JSON Import - View Basic]( http://va3c.github.io/viewer/cookbook/r1/json-import-view-basic.html )   
Source code: [JSON Import - View Basic](  https://github.com/va3c/viewer/tree/gh-pages/cookbook/r1/json-import-view-basic.html )

This file has a single command: "Select File' brings up your operating system's file dialog. You can select any file,
but a good place to start is with the file you just exported.

Once loaded, the file allows you to zoom, pan and rotate. Attribute values - assigned to the entire mesh - may also appear just under the File select button.

Again, this script is designed to be simple and basic in order t give you the quickest feeling of hos things work.

Now that you have viewed the export and import process, it is time to add a bit more complexity.

Live demo: [JSON Build - Export Object]( http://va3c.github.io/viewer/cookbook/r1/json-build-export-object.html )  
Source code: [JSON Build - Export Object](  https://github.com/va3c/viewer/tree/gh-pages/cookbook/r1/json-build-export-object.html )

This script extrudes a shape and therefore the geometry is more complicated than the first example. 
Therefore Three.js exports all the vertices and faces.

This script also exports more meta information - including any materials that have been assigned to the geometry.

This type of data is likely to be far closer to the type of data you will likely be exporting from your app.

**

Coming next

* Text and numeric attributes attached to individual faces
* Colors assigned to individual faces


Remember: the JavaScript console is your friend...

### Mission  
<!-- a statement of a rationale, applicable now as well as in the future -->



### Vision  
<!--  a descriptive picture of a desired future state -->


## Features
<!-- and benefits -->


## Road Map


## Issues / Bugs


## Project Links
vA3C is a [GitHub]( http://github.com) [organization account]( https://help.github.com/articles/what-s-the-difference-between-user-and-organization-accounts ) and has multiple owners and admins. 
All vA3EC scripts are [FOSS]( https://en.wikipedia.org/wiki/Free_and_open-source_software ).
Scripts are hosted on GitHub and are viewable as web pages, as described in the 'Read Me' files and as source code.

The three ways of looking at the vA3C scripts:

1. [Live Demo]( http://va3c.github.io/viewer/cookbook/r1/json-build-export-object.html )  
2. [Read Me]( http://va3c.github.io/viewer/cookbook "view the files as apps." ) <input value="<< You are now probably here." size=28 style="font:bold 12pt monospace;border-width:0;" >   
3. [Source Code]( https://github.com/va3c/viewer/tree/gh-pages/cookbook "View the files as source code." ) <scan style=display:none ><< You are now probably here.</scan>  


## System Requirements

In order to run the script you will need a device and browser that provides good support for [WebGL](http://get.webgl.org/)
WebGL is the JavaScript API for rendering interactive 3D graphics and 2D graphics within any compatible web browser without the use of plug-ins. 

Generally this means a computer with an Intel Core i5 processor or better with an external GPU such as one made by Nvidia. 
Successful use of the script on a phone or tablet is highly unlikely. 
A mouse or other pointing device with a scroll wheel is also highly recommended so that you can zoom, pant and rotate in 3D.
 
The script is currently being built and tested with the Google Chrome browser. 
Bugs on browsers other than Chrome need not be reported until such time as the work settles down and an effort to support more browsers is initiated.


## Copyright and License

copyright &copy; 2014 vA3C authors ~ 
All work herein is under the [MIT License]( http://jaanga.github.io/libs/jaanga-copyright-and-mit-license.md )

This repository contains files that are at an early and volatile stage. Not all licensing requirements may have been fully met let alone identified. It is the intension of the authors to play fair and all such requirements will either be met or the feature in question will turned off.


## Change Log

2014-06-26 ~ Add folders and files 

