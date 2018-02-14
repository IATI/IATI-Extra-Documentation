Example Usage
~~~~~~~~~~~~~
Example ``description`` of an ``iati-activity``.

| The ``@type`` attribute declares a valid code (*en*) from the *DescriptionType* codelist.

.. code-block:: xml

    <description type="1">
       <narrative>General activity description text.  Long description of the activity with no particular structure.</narrative>
    </description>

| The ``description`` element can be repeated in any ``iati-activity``.
| In this example, three different ``description`` are declared.
| Note - it is optional to include all ``DescriptionType``.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--description starts-->
	:end-before: <!--description ends-->

Changelog
~~~~~~~~~
2.01
^^^^
| Freetext is no longer allowed with this element.  It should now be declared with the new child ``narrative`` element.
