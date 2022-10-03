GroupItem
=========

=======
Summary
=======

A **GroupItem** is responsible for keeping track of
all the **:doc:`blockItem`** objects and the order they are in.

A group combines a logical ordering of "screens" and the order in which they
should be displayed.  For example, a group may contain one passage,
and ten questions.


Declaration
-----------

.. code-block:: swift

   struct GroupItem

Properties
----------------

**id**: *String*
  The unique identifier for the **GroupItem** item.

**blockOrder**: *Array<:doc:`blockItem`>*
  An array of :doc:`key` values that track the order of :doc:`blockItem`
