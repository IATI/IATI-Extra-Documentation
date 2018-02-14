Example Usage
~~~~~~~~~~~~~
Example ``contact-info`` for an ``iati-activity``.

| This element is a parent for other child elements.

| The ``@type`` attribute declares a valid code (*1*) from the *ContactType* codelist.

.. code-block:: xml

	<contact-info type="1">
	...
	</contact-info>

| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--contact-info starts-->
	:end-before: <!--contact-info ends-->

Changelog
~~~~~~~~~

2.01
^^^^
The optional ``contact-info/department`` element was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#contact-info-department-new-element>`__.

1.03
^^^^
Added the optional ``contact-info/website`` element.

| Added the optional ``contact-info/@type`` attribute.

| Changed the following subelements of contact-info to allow multiple-language versions explicitly (no change to parsing; purely semantic):

-  organisation
-  person-name
-  job-title
-  mailing-address
