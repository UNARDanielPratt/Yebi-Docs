BarData
=======

=======
Summary
=======

*BarData* contains bar graph data for a single bar.

Properties
----------------

**id**: :doc:`/key`
  The UID of the *BarData* item.

**category**: :doc:`/textitem` 
  The name of a category for this bar data.  All bars with
  the same group title name will be grouped together.
  For example, if a bar graph describes how people click on a link,
  the categories could be "first time visitor", "returning visitor".

**group**: :doc:`/textitem` 
  The name for the value that this data represents.
  Extending the example from above the group names
  for the data could be "2019", "2020", "2021" etc.

**value**: *Float*
  The numerical value for this data point.
