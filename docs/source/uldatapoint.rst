ULDataPoint
===========

=======
Summary
=======

A data structure that keeps track of important data points
inside of a :doc:`/cartesianitem`.

Properties
-----------

**color**: :doc:`/ulcolor`
  The color this point should be drawn with.

**pointSize**: *Float*
  The size the point needs to be drawn with.

**touchType**: *Int*
  The type of feedback to give for this line item
  TODO: A touchType enum needs to be created.

**locations**: Array<:doc:`/ulpoint`>
  An array of the points to be drawn.
