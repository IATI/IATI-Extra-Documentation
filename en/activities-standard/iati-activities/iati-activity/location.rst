

Example Usage
~~~~~~~~~~~~~

The location element is used a contain various other elements

.. code-block:: xml

        <location>
           ....
        </location>

If more than one location is reported, percentage of activity commitment
allocated to this location (if available).

.. code-block:: xml

        <location percentage="85>
           ....
        </location>
        <location percentage="15>
           ....
        </location>

Example:

.. code-block:: xml

    <location>
          <name>Herat</name>
          <coordinates latitude="34.341944400000003000" longitude="62.203055599999971000" precision="2" />
          <location-type code="PPL" />
          <administrative country="AF">Afghanistan, Herat, Injil</administrative>
        </location>

Changelog
~~~~~~~~~

1.04
^^^^
|The @ref attribute was introduced to provide a cross reference that a publisher can use to link back to their own internal system.
|The @percentage attribute was deemed unworkable and deprecated in 1.04


1.03
^^^^

Where used, the @percentage attribute is now designated as a decimal
value and no longer as a positive Integer
