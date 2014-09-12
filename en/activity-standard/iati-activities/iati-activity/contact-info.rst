Example Usage
~~~~~~~~~~~~~
Example ``contact-info`` for an ``iati-activity``.

| This element is a parent for other child elements.

| This example declares ``ContactType`` code *1* (*General Enquiries*) with the ``type`` attribute.

.. code-block:: xml

	<contact-info type="1">
	...
	</contact-info>

| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--contact-info starts-->
	:end-before: <!--contact-info ends-->
	:emphasize-lines: 1, 20

Changelog
~~~~~~~~~

1.03
^^^^

Added the optional contact-info/website element

Added the optional contact-info/@type attribute

Changed the following subelements of contact-info to allow multiple-language versions explicitly (no change to parsing; purely
semantic):

-  organisation
-  person-name
-  job-title
-  mailing-address
