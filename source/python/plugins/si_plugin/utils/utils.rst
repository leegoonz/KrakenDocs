Utils
*****

The Softimage Kraken plug-in utils.


Modules
=======

.. toctree::
   :maxdepth: 2
   :titlesonly:

   /python/plugins/si_plugin/utils/curves


Module Data
===========

.. py:data:: si

   Softimage Application

.. py:data:: sel

   Softimage Selection

.. py:data:: log

   Softimage Log Command

.. py:data:: XSIMath

   Softimage Math Utility Library

.. py:data:: XSIUtils

   Softimage Utility Library

.. py:data:: XSIUIToolkit

   Softimage UI Toolkit Library

.. py:data:: XSIFactory

   Softimage Factory Library


Module Methods
==============

.. py:method:: getCollection()

   Returns an XSICollection object.


.. py:method:: lockObjXfo(dccSceneItem):

   Locks the dccSceneItem's transform parameters.

   :param object dccSceneItem: DCC object to lock transform parameters on.

   :return: True if successful.
   :rtype: bool


.. contents:: Usage Documentation
   :local:


.. include:: ../../../../footer.rst