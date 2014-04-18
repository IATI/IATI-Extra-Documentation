Example Usage
~~~~~~~~~~~~~

Example of an ``iati-activity`` with one each of the four possible ``ActivityDateType``:

.. code-block:: xml

    <activity-date iso-date="2012-04-15" type="start-planned">2012-04-15</activity-date>
    <activity-date iso-date="2012-04-28" type="start-actual">2012-04-28</activity-date>
    <activity-date type="end-planned" iso-date="2013-10-31">2013-10-31</activity-date>
    <activity-date type="end-actual" iso-date="2013-12-31">2013-12-31</activity-date>

In some cases, not all ``activity-date`` can be declared, depending on the ``activity-status`` of the ``iati-activity``:

.. code-block:: xml

    <activity-date iso-date="2012-04-15" type="start-planned">2012-04-15</activity-date>
    <activity-date iso-date="2012-04-28" type="start-actual">2012-04-28</activity-date>
    <activity-date iso-date="2015-12-31" type="end-planned">2015-12-31</activity-date>
        
Note: a ``start-actual`` or ``end-actual`` with a date in the *future*, is not expected.
