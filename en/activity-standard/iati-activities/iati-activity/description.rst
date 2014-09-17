Example Usage
~~~~~~~~~~~~~
Example ``description`` of an ``iati-activity``.

.. code-block:: xml

	<description type="1">
       <narrative>General activity description text.  Long description of the activity with no particular structure.</narrative>
    </description>


| The ``description`` element can be repeated in any ``iati-activity``.
| In this example, different ``description`` are declared.
|
| A ``DescriptionType`` code is declared for each, using the ``type`` attribute.

| Note - it is optional to include all ``DescriptionType``:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--description starts-->
	:end-before: <!--description ends-->
	:emphasize-lines: 1, 4, 5, 8, 9, 12
