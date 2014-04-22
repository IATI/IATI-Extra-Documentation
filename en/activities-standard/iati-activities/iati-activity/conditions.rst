Example Usage
~~~~~~~~~~~~~
The ``conditions`` element acts as a container for other sub elements. 

It is declared through a boolean value (*0*=no, *1!=yes) stating whether there are ``conditions`` attached to the ``iati-activity``:

For when no conditions are attached to the ``iati-activity``:

.. code-block:: xml

    <conditions attached="0"/>

For when conditions are attached to the ``iati-activity``

.. code-block:: xml

    <conditions attached="1">
    ...
    </conditions>

Full example of ``conditions`` attached:

.. code-block:: xml

    <conditions attached="1">
      <condition type="1">Conditions text</condition>
    </conditions>
