PassageItem
===========

=======
Summary
=======

A **PassageItem** represents a multiline block of text.

Properties
----------------

**id**: :doc:`key`
  The unique identifier for the **PassageItem** item.

**sequenceItems**: [:doc:`/blockitem`]
  An array of :doc:`/blockitem` items that point at individual
  :doc:`/textitem` and :doc:`/equationitem` values that come
  before the main *textContent*.

**textContent**: *String*
  The entire text that the **PassageItem** contains.

**lines**: [:doc:`ulspan`]
  Spans of all the lines as parsed via OCR from the original physical document.

**sentences**: [:doc:`ulspan`]
  Spans of all the sentences contained in the *textContent* string.

**underlines**: [:doc:`ulspan`]
  Spans of any underlined items in the *textContent* string.

**paragraphs**: [:doc:`ulspan`]
  Spans of all the paragraphs contained in the *textContent* string.
  .. note:: At the very least, this will contain the start and end index of the *textContent*
