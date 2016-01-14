Logger
******


.. contents:: Usage Documentation
   :local:


Class Documentation
===================

.. py:class:: OutputLog(object)

   Output messages and errors are stored in this object and can be recalled when creating widgets that need to show the history of messages and errors.

   .. py:method:: __init__(self)

   .. py:method:: write(self, text)

   .. py:method:: getLog(self)

      Gets the logged output to this point.

      :returns: Logged output.
      :rtype: str


.. include:: ../../../footer.rst