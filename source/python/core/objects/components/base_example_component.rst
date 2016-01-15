Base Example Component
**********************


.. contents:: Usage Documentation
   :local:


Overview
========

This base component automatically sets up a hierarchy which includes a control :doc:`/python/core/objects/layer` with a :doc:`/python/core/objects/hierarchy_group` for inputs and one for outputs. This is done for convenience to have a base component setup to not only demonstrate how to create a default hierarchy but also to demonstrate how to setup the attach and detach methods.

The :py:meth:`~.BaseExampleComponent.attach` and :py:meth:`~.BaseExampleComponent.detach` are methods that are only invoked through the user interface. Since components can be dynamically added and removed from a :doc:`/python/core/objects/container` through the UI, these methods are necessary in order keep the graph clean.


Class Documentation
===================

.. autoclass:: kraken.core.objects.components.base_example_component.BaseExampleComponent
    :members:
    :private-members:
    :special-members:
    :undoc-members:
    :show-inheritance:
    :exclude-members: __module__


.. include:: ../../../../footer.rst