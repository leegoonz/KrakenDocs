############
Installation
############

.. contents::
   :local:

|

Prerequisites
*************
* Python 2.7.x
* PySide 1.2.2

|

Download
********
https://github.com/fabric-engine/Kraken

|

Environment Variables
*********************
|

.. glossary::

   KRAKEN_DIR
      Base directory where Kraken is installed.

   KRAKEN_PATHS
      Paths to custom components.

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

   set FABRIC_DIR=D:\fabric\FabricEngine-1.15.2-Windows-x86_64

   set KRAKEN_DIR=D:\dev\kraken

   set PATH=%FABRIC_DIR%\bin;%PATH%

   set FABRIC_EXTS_PATH=%FABRIC_DIR%\Exts;%FABRIC_EXTS_PATH%;%KRAKEN_DIR%\KLExts;

   set PYTHONPATH=%PYTHONPATH%;%FABRIC_DIR%\Python\2.7;%KRAKEN_DIR%\Python;


   cd /d D:\dev\kraken\Python\kraken

   call cmd


Windows Softimage 2015
======================
|

.. highlight:: bash

::

   set FABRIC_DIR=D:\fabric\FabricEngine-1.15.2-Windows-x86_64

   set KRAKEN_DIR=D:\dev\kraken

   set PATH=%FABRIC_DIR%\bin;%PATH%

   set FABRIC_EXTS_PATH=%FABRIC_DIR%\Exts;%FABRIC_EXTS_PATH%;%KRAKEN_DIR%\KLExts;

   set PYTHONPATH=%PYTHONPATH%;%FABRIC_DIR%\Python\2.7;%KRAKEN_DIR%\Python;


   call "C:\Program Files\Autodesk\Softimage 2015 SP1\Application\bin\XSI.bat"

   echo OFF


Windows Maya 2015
=================
|

.. highlight:: bash

::

   set FABRIC_DIR=D:\fabric\FabricEngine-1.15.2-Windows-x86_64

   set KRAKEN_DIR=D:\dev\kraken

   set PATH=%FABRIC_DIR%\bin;%PATH%

   set FABRIC_EXTS_PATH=%FABRIC_DIR%\Exts;%FABRIC_EXTS_PATH%;%KRAKEN_DIR%\KLExts;

   set PYTHONPATH=%PYTHONPATH%;%FABRIC_DIR%\Python\2.7;%KRAKEN_DIR%\Python;


   set MAYA_MODULE_PATH=%FABRIC_DIR%\SpliceIntegrations\FabricSpliceMaya2015SP2;%KRAKEN_DIR%\DCCIntegrations\maya;

   start /d "C:\Program Files\Autodesk\Maya2015\bin" maya.exe


.. include:: footer.rst