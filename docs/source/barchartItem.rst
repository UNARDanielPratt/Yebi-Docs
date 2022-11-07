BarchartItem
============

=======
Summary
=======

A **BarchartItem** is a data structure that represents a bar chart.

Properties
----------------

**id**: :doc:`key`
  The unique identifier for the **BarchartItem** item.

**aspectRatio**: *Int*
    A decimal representation of aspect ratio (width/height)
    used in reproducing the graphic.

**data**: Array<:doc:`bardata`>
  An array of data points for the graph.

**description**: *String*
  A human understandable description of this figure.

**figureTitle**: :doc:`/textitem` **Optional**
  The title of the figure.

**xAxisLabel**: :doc:`/textitem`  **Optional**
  The label that describes the x axis.

**yAxisLabel**: :doc:`/textitem`  **Optional**
  The label that describes the y axis.
