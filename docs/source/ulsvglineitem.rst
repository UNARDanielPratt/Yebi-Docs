ULSvgLineItem
=============

=======
Summary
=======

A line of svg data that is used to draw an image.

Properties
------------

**id**: :doc:`key`
  A unique identifier for this item.
  Note: This is used to help saving edited data.

**isClosed**: *Boolean*
  Informs if the shape should be closed or not.

**dashPatternType**: :doc:`/uldashpattern`
  The type of dash pattern to drawn.
  Note: (enum item 0 is just a normal line with no dashes).

**line**: Array<:doc:`/ulsvgdata`>
  The point or points that inform this svg line instruction.

**shapeType**: :doc:`/shapetype` *Optional*
  The type of shape this is (helps with drawing).

**color**: :doc:`/ulcolor` *Optional*
  The stroke color that this path should be drawn with.

**strokeWidth**: *Float*
  The stroking width that the line should be drawn with

**touchType**: *Int*
  The type of feedback to give for this line item
  TODO: A touchType enum needs to be created.
