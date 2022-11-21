CartesianItem
=============

=======
Summary
=======

A **CartesianItem** is a data structure that represents a cartesian
chart with lines and curves in a four quadrant grid.

Properties
------------

**id**: :doc:`key`
  The unique identifier for the **CartesianItem** item.

**dataCurves**: Array<:doc:`/ulsvglineitem`>
  Contains SVG data used to draw graph lines.

**dataPoints**: Array<:doc:`/uldatapoint`> *Optional*
  Points of interest on the graph.

**aspectRatio**: *Int*
    A decimal representation of aspect ratio (width/height)
    used in reproducing the graphic.

**description**: *String*
  A human understandable description of this figure.

**topTitle**: :doc:`key` **Optional**
  The unique id for the :doc:`/textitem` that describes the
  title displayed above the graph.

**xTitle**: :doc:`key` **Optional**
  The unique id for the :doc:`/textitem` that describes the
  title displayed below the graph along the x-axis.

**yTitle**: :doc:`key` **Optional**
  The unique id for the :doc:`/textitem` that describes the
  title displayed to the left of the graph along the y-axis.

**textItems**: *Dictionary* <:doc:`key` : :doc:`/textitem`>
  A dictionary that contains the titles and labels associated
  with this graph.  The dictionary key is the UID of the
  :doc:`/textitem`, and the value is the :doc:`/textitem`
  iteself.

**xOffset**: *Float*
  The offset (0-value) location for the x-axis.

**yOffset**: *Float*
  The offset (0-value) location for the y-axis.

**xScale**: *Float*
  The scaling used to calculate values for the x-axis.

**yScale**: *Float*
  The scaling used to calculate values for the y-axis.

**xLabels**: Array<:doc:`key`>
  The values associated with the various ticks along
  the x-axis.  This array MUST be the same length as
  the *xTicks* array.

**xTicks**: Array<*Float*>
  An array of floats that describe placement of vertical
  grid lines along the x-axis.  The values are normalized
  x-coordinates, so the range should be from 0.0-1.0.

**yLabels**: Array<:doc:`key`>
  The values associated with the various ticks along
  the y-axis.  This array MUST be the same length as
  the *yTicks* array.

**yTicks**: Array<*Float*>
  An array of floats that describe placement of horizontal
  grid lines along the y-axis.  The values are normalized
  y-coordinates, so the range should be from 0.0-1.0.
