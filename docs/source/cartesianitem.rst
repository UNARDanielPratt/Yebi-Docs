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

**xOffset**: *Float*
  The offset (0-value) location for the x-axis.

**yOffset**: *Float*
  The offset (0-value) location for the y-axis.

**xScale**: *Float*
  The scaling used to calculate values for the x-axis.

**yScale**: *Float*
  The scaling used to calculate values for the y-axis.

**numXGridLines**: *Int* *Optional*
  The number of grid lines to try to draw along the x-axis.

**numYGridLines**: *Int* *Optional*
  The number of grid lines to try to draw along the y-axis.
