ULSvgLineType
=============

=======
Summary
=======

The type of svg instruction being given.

Enum Values
------------

**move**: *0*
  Instruction to move draw location to given coords without
  drawing.

**quadratic**: *1*
  Instruction to add a quadradic curve at given point and control.

**line**: *2*
  Instruction to draw a line from last point to given point.

**end**: *3*
  Instruction that informs drawing of this shape has ended.
