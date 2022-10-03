ContextItem
===========

=======
Summary
=======

A **ContextItem** is a structure used to link to a specific span
contained inside a :doc:`/passageitem`

Using the start and end indexes, a new string may be formed from the
referenced :doc:`/passageitem`. For instance, if the referenced
:doc:`/passageitem` has the *textContent* "Hello, World!" and this
*ContextItem* has a start of *0* and an end of *4* you will be able to
extract the string "Hello" from the original :doc:`/passageitem`.

Properties
----------------

**id**: :doc:`key`
  The unique identifier for the **ContextItem** item.

**passageItemId**: :doc:`key`
  The unique identifier for the :doc:`/passageitem` being referenced.

**start**: *Int*
  The index of the starting character inside the referenced :doc:`/passageitem`

**end**: *Int*
  The index of the ending character inside the referenced :doc:`/passageitem`
