TableItem
===========

=======
Summary
=======

A **TableItem** represents a table graphic item.

.. note::
    This structure is not sufficient for providing useful information
    to VoiceOver users.  See the proposed data structure below the main
    definition for an explination of how future versions may be implemented.

Properties
-----------

**id**: :doc:`key`
  The unique identifier for the *TableItem* item.

**aspectRatio**: *Float*
  The aspect ratio (width / height) as represented by a decimal number.

**description**: *string*
  A human readable description of the graphic.

**equationItems**: [:doc:`/equationitem`]
  Array of all the :doc:`/equationitem` objects used to render table.

**textItems**: [:doc:`/textitem`]
  Array of all the :doc:`/textitem` objects used to render table.

**table**: [:doc:`/ultabledata`]
  The data values that are used to draw the table.

================
Proposed Updates
================

Abstract
---------

The current version of the structure allows for succesful visual rendering
of pretty much any type of table, but it does not allow for useful navigation
by VoiceOver users.  By boiling a table down to the actual information it
contains, rather than thinking first about how it is rendered, we are able
to store table data in a way that will allow VoiceOver users to more easily
understand and navigate a table.

By associating values in a 2d-matrix, we are able to easily associate a value
with relevent header information.

Proposed Properties
--------------------

Root Table Object
-----------------

**type**: *Enum*
  An enum that would describe what type of chart this is.
  (e.g. single-header, two-header, irregular-headers)

**x-headers**: [*Header*]
  An array of header structures (more on that below)
  that contain the x-direction column header values.

**y-headers**: [*Header*]
  An array of header structures (more on that below)
  that contain the y-direction column header values.

**values**: *2D Matrix*
  A 2-D matrix array that contain the actual values
  for table cells.

Header Structure
----------------

**title**: *String*
  A string representing the actual contents of the cell.
  This may need to be a more complicated item representation.
  (e.g. may need to point to the uid of a :doc:`/textitem`)

**subHeaders**: [*Header*]
    A header may contain subheaders.
    For an example of a table with this type of irregular header
    see `this link <https://www.w3.org/WAI/tutorials/tables/irregular/>`_

