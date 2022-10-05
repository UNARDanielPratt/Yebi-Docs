ULSpan
===========

=======
Summary
=======

A **ULSpan** keeps track of the start and end indexes of an item.

Properties
----------------

**id**: :doc:`key`
  The unique identifier for the **ULSpan** item.

**start**: *Int*
  The starting index of the span.

**end**: *Int*
  The ending index of the span.

**inParagraph**: :doc:`/key` *optional*
  The UID of the paragraph (if any) that this span is found inside of.
  This is optional, and should never be included if the span is
  describing the paragraph itself.
