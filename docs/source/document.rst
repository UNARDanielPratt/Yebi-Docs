Document
========

=======
Summary
=======

This structure represents a converted document.

Declaration
-----------

.. code-block:: swift

   struct Document

Properties
----------------

**id**: :doc:`key`
The unique identifier for this document.

**status**: *Double*
  This number tracks the percentage of the document that has been
  converted by the backend.

  Values range from 0.0 to 1.0.  A value of -1 means it has failed.

**createdDate**: `TimeStamp <https://firebase.google.com/docs/reference/unity/struct/firebase/firestore/timestamp>`_
  This is the date the document was created on, it is stored as a
  Firestore TimeStamp.

