############
Installation
############

.. contents::
   :local:

|

Pre-Requisites
**************
* Fabric Engine 1.15.3
* Python 2.7.x
* PyWin32 (Softimage requirement)
* PySide
* PyQtForSoftimage (PySide compatible version)

|

Download
********
Get the latest version of Kraken here:
`Kraken Downloads <http://fabric-engine.github.io/Kraken/#download>`_

|

DCC Installation
****************

|

Softimage Installation
======================
Once the pre-requisites have been installed, you need to connect to a few workgroups.

The order of the workgroups should be:

1. Fabric Engine
2. PyQtForSoftimage
3. Kraken

|

Maya Installation
=================
Once the pre-requisites have been installed, you need to add Fabric and Kraken to the MAYA_MODULE_PATH. See the example launcher script below or see teh Maya documentation on how to add paths to the MAYA_MODULE_PATH.

Once added, you'll have to activate the plug-ins by going to Window > Settings / Preferences > Plug-in Manager. There you should activate:

1. FabricSplice.mll
2. kraken_maya.py

|

Environment Variables
*********************
|

.. glossary::

   KRAKEN_PATH
      Base directory where Kraken is installed.

   KRAKEN_PATHS
      Paths to custom components and configs.

   KRAKEN_LOAD_MENU
      If set to False, the Kraken Menu will not load in the DCC's. However the commands will still be registered.

|

Example Launcher Scripts
************************
|

Windows Standalone
==================
|

.. highlight:: bash

::

   set KRAKEN_PATH=D:\fabric\FabricEngine-1.15.2-Windows-x86_64

   set KRAKEN_DIR=D:\dev\kraken

   set PATH=%KRAKEN_PATH%\bin;%PATH%

   set FABRIC_EXTS_PATH=%KRAKEN_PATH%\Exts;%FABRIC_EXTS_PATH%;%KRAKEN_DIR%\KLExts;

   set PYTHONPATH=%PYTHONPATH%;%KRAKEN_PATH%\Python\2.7;%KRAKEN_DIR%\Python;


   cd /d D:\dev\kraken\Python\kraken

   call cmd


Windows Softimage 2015
======================
|

.. highlight:: bash

::

   set KRAKEN_PATH=D:\fabric\FabricEngine-1.15.2-Windows-x86_64

   set KRAKEN_DIR=D:\dev\kraken

   set PATH=%KRAKEN_PATH%\bin;%PATH%

   set FABRIC_EXTS_PATH=%KRAKEN_PATH%\Exts;%FABRIC_EXTS_PATH%;%KRAKEN_DIR%\KLExts;

   set PYTHONPATH=%PYTHONPATH%;%KRAKEN_PATH%\Python\2.7;%KRAKEN_DIR%\Python;


   call "C:\Program Files\Autodesk\Softimage 2015 SP1\Application\bin\XSI.bat"

   echo OFF


Windows Maya 2015
=================
|

.. highlight:: bash

::

   set KRAKEN_PATH=D:\fabric\FabricEngine-1.15.2-Windows-x86_64

   set KRAKEN_DIR=D:\dev\kraken

   set PATH=%KRAKEN_PATH%\bin;%PATH%

   set FABRIC_EXTS_PATH=%KRAKEN_PATH%\Exts;%FABRIC_EXTS_PATH%;%KRAKEN_DIR%\KLExts;

   set PYTHONPATH=%PYTHONPATH%;%KRAKEN_PATH%\Python\2.7;%KRAKEN_DIR%\Python;


   set MAYA_MODULE_PATH=%KRAKEN_PATH%\SpliceIntegrations\FabricSpliceMaya2015SP2;%KRAKEN_DIR%\DCCIntegrations\maya;

   start /d "C:\Program Files\Autodesk\Maya2015\bin" maya.exe


.. include:: footer.rst