Block
=========

=======
Summary
=======

A **Block** is responsible for keeping track of
all the content that is on a single screen of content.

Properties
----------------

**id**: :doc:`key`
  The unique identifier for the **GroupItem** item.

**blockType**: :doc:`blocktype`
  The type of block this **BlockItem** represents.

**questionNumber**: :doc:`key` *optional*
  The UID of a :doc:`/textitem` that contains the question question
  number related to this question.  (Will be null for all non-question items).

**items**: [:doc:`/blockitem`]
  An array of the main content of the passage or the question being asked.

**options**: [:doc:`/optionitem`]
  An array of available options associated with a question.
  This array will be empty for all non-question type blocks.

**solutionIndex**: *Int*
  The index of the correct answer in the *options* array.
  If no answer is known, this is set to -1.

**context**: :doc:`key` *optional*
  If a block references a span of text in a :doc:`/passageitem`,
  this will contain a key that points at the :doc:`/contextitem` that contains
  the related information.

  (e.g. A question references lines 1-3 from the passage, *context*
  will point at the :doc:`/contextitem` that defines the text to be displayed).
