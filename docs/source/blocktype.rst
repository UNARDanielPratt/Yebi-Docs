BlockType
==========

=======
Summary
=======

An *Int* typed enum that representes the different section types.

===========
Enum Values
===========

| **context**: *0*
  A block item that references an item that is of the **Context** type.
  This type is most likely a :doc:`/passageitem`.

**question**: *1*
  A block item that references some kind of question.
  (e.g. A math problem with 4 possible answer options).

**info**: *2*
  A block that references some type of instructions.

**unknown**: *-1*
  A block that the backend was unable to indentify the type of.
  This type will be ignored by the frontend completely.
