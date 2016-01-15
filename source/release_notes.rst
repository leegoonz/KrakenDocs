=============
Release Notes
=============


*************
Version 1.1.0
*************

*Released 2016-01-15*


New Features
   * Added sample .bat launcher files. ``extras``
   * Core graph code extracted to PyflowGraph repo and added as a sub-tree. ``ui``
   * Backdrops have been added for grouping nodes. ``ui``
   * Add Color Attribute ``core``
   * Control object needs method "setShape". ``core``
   * Ability to refresh the Component list manually. ``core`` ``ui``
   * Use resource file for images. ``ui``
   * Snap to Grid. ``ui``
   * Node color should be taken from component .py files. ``ui``
   * Add Recent Files Menu. ``ui``


Fixed
   * Kraken Maya plugin auto loads matrixNodes plugin automatically now. ``Maya``
   * Spine pop fix. ``solvers``
   * Doing Save As doesn't update file path in title bar. ``ui``
   * Kraken UI won't open if one kraken path not found. ``ui``
   * Kraken UI Slow, and slowing the host UI. ``ui``


Changed
   * Use KRAKEN_PATH instead of KRAKEN_DIR in core and in launcher scripts. ``core``
   * Component Library widget to folder tree widget. ``ui``
   * Tracks opened file, save command simply saves file. ``ui``
   * When doing a save as / open, file name isn't stored or restored next time. ``ui``
   * Output log widget added to allow users to see the history. ``ui``
   * Error message is now full length of window and stays on screen longer. ``ui``
   * Renamed KLExts and DFG folders to be consistent with how core Fabric Engine nodes are organized. ``core``


*************
Version 1.0.0
*************

*Released 2015-08-11*



.. include:: footer.rst