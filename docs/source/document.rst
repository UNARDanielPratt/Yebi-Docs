Document
========

.. _document_summary:

=======
Summary
=======

This structure represents a converted document.

.. _document_declaration:

Declaration
-----------

.. code-block:: swift

   struct Document

Properties
----------------

**id**: *String*
The unique identifier for this document.

**status**: *Double*
  This number tracks the percentage of the document that has been converted by the backend.

  Values range from 0.0 to 1.0.  A value of -1 means it has failed.

**createdDate**: *TimeStamp*
  This is the date the document was created on, it is stored as a Firestore TimeStamp.

