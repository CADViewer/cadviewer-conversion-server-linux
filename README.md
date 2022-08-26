# Installing CADViewer NodeJS Conversion Server - Linux

The CADViewer NodeJS Conversion server on Linux (/opt/cadviewer-conversion-server/) is used in six different implementations: **NodeJS**, **Angular**,**ReactJS**, **Laravel**, **Rails7** and **VueJS**. 

The repository contains a full setup including converters and NodeJS controlling script


## This package contains

1: NodeJS script library for controlling CAD Conversions and communication with CADViewer  - in its preferred folder structure

2: AutoXchange AX2023 Converter, DWG Merge 2023 Converter and LinkList 2023 Converter - in their preferred folder structure

3: All structures for file-conversion, sample drawings, redlines, etc. 


## This package does not contain

4: The converter folder structure contains a larger set of fonts, installed in /cadviewer/converters/ax2023/windows/fonts/, but a fuller set of fonts can be installed. 

Read the sections on installing and handling [Fonts](https://tailormade.com/ax2020techdocs/installation/fonts/) in [AutoXchange 2023 TechDocs](https://tailormade.com/ax2020techdocs/) and [TroubleShooting](https://tailormade.com/ax2020techdocs/troubleshooting/).



## How to Use


1: Ensure that all paths and ports are set correctly in ***CADViewer_config.json***, we use port 3000 as standard, but the given setup or framework may require a different setting. 

2: Depending on the implementation, ServerFrontEndUrl may change. 


3:  Ensure that all executables have chmod 777 permission and that the /converters/files folder has full read and write permission also. 

4: This install includes the AutoXchange 2023 converter, but if needed, it can be updated from our [download](https://cadviewer.com/download) resources.

5: The [CADViewer](https://cadviewer.com/cadviewertechdocs) front-end can be found from our [download](https://cadviewer.com/download) resources, or installed directly from npm with: **npm i cadviewer**.

6: See [Business Extensions to Handlers](https://cadviewer.com/cadviewertechdocs/handlers_business/) and [CADViewer RESTFUL API](https://cadviewer.com/cadviewertechdocs/rest_api/) to extend the back-end with a customExtension for reading of Blobs/internal datastructure, etc. 



**NOTE:** Make sure the converter version number in CADViwer_config.json match the converters you install, and change any paths settings to correspond to your install folders.  

**Run:** the NodeJS server with:  *node CV_7.x.yy*



## General Documentation 

-   [CADViewer Techdocs and Installation Guide](https://cadviewer.com/cadviewertechdocs)



## Updating CAD Converters

This repository should contain the latest converters, but in case you need to update any of the back-end converters please follow: 

* [Download **AutoXchange**](/download/) (and other converters), install (unzip) AX2023 in **cadviewer/converters/ax2023/windows** or **cadviewer/converters/ax2023/linux** or in the designated folder structure.

* Read the sections on installing and handling [Fonts](https://tailormade.com/ax2020techdocs/installation/fonts/) in [AutoXchange 2023 TechDocs](https://tailormade.com/ax2020techdocs/) and [TroubleShooting](https://tailormade.com/ax2020techdocs/troubleshooting/).

* Try out the samples and build your own application!
 
 

