Example Usage
~~~~~~~~~~~~~
Example ``location`` for an ``iati-activity``.

| This element is a parent for other child elements.

| An example organisation ``@ref`` of *AF-KAN* is declared.

.. code-block:: xml

	<location ref="AF-KAN">
	...
	</location>

| Full example with all child elements:    
    
.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->
	:emphasize-lines: 1, 20

| The ``location`` element can be repeated in any ``iati-activity``.

Changelog
~~~~~~~~~

1.04
^^^^

Note that major changes were made to the subelements of ``location`` in version 1.04.  

| For more information refer to: 

* the :doc:`1.04 location changes overview guidance </upgrades/decimal-upgrade-to-1-04/location-summary/>`
* the :ref:`Activities Schema Changelog <1_04_activities_schema_changes>` (or the individual subemelement pages)

| The @ref attribute was introduced to provide a cross reference that a publisher can use to link back to their own internal system.
| The @percentage attribute was deemed unworkable and deprecated in 1.04


1.03
^^^^

Where used, the @percentage attribute is now designated as a decimal
value and no longer as a positive Integer
