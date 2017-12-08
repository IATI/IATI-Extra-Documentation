Example Usage
~~~~~~~~~~~~~
Example ``default-aid-type``  for an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*A01*) from the *AidType* codelist.
| The ``@vocabulary`` attribute declares a code for the vocabulary aid-type classifications to define the ``@code`` value unless omitted.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--default-aid-type starts-->
	:end-before: <!--default-aid-type ends-->

Changelog
~~~~~~~~~

2.03
^^^^
``@vocabulary attribute added <add link here> to this element.

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.
