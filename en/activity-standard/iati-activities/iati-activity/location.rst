Example Usage
~~~~~~~~~~~~~
The ``location`` element is used a contain various other elements

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->


Changelog
~~~~~~~~~

1.04
^^^^

Note that major changes were made to the subelements of ``location`` in version 1.04, see the :ref:`Activities Schema Changelog <1_04_activities_schema_changes>` (or the individual subemelement pages) for more information.

| The @ref attribute was introduced to provide a cross reference that a publisher can use to link back to their own internal system.
| The @percentage attribute was deemed unworkable and deprecated in 1.04


1.03
^^^^

Where used, the @percentage attribute is now designated as a decimal
value and no longer as a positive Integer
