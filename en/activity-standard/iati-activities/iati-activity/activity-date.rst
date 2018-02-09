Example Usage
~~~~~~~~~~~~~
Example ``activity-date`` for an``iati-activity``.

| The ``@type`` attribute declares a valid code (*1*) from the *ActivityDateType* codelist.

| An example date is declared in the ``@iso-date`` attribute.
| Example date format conforms to the *xsd:date* standard - for most cases *YYYY-MM-DD* is sufficient.

.. code-block:: xml

	<activity-date iso-date="2012-04-28" type="1" />

| The ``activity-date`` element can be repeated in any ``iati-activity``.
| In this example four ``activity-date`` are declared.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--activity-date starts-->
	:end-before: <!--activity-date ends-->

Note: In some cases, not all *ActivityDateType* codes can be declared, depending on the ``activity-status`` of the ``iati-activity``

| Note: All instances of the *ActivityDateType* code *2* & *4* (actual dates) are not expected to be in the *future*.

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element.

| The ``ActivityDateType`` codelist was changed to numeric codes


