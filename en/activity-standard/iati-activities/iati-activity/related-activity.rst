Example Usage
~~~~~~~~~~~~~
Example ``related-activity`` of an ``iati-activity``.

| The ``@type`` attribute declares a valid code (*1*) from the *RelatedActivityType* codelist.
| An example ``@ref`` for another ``iati-activity`` of *AA-AAA-123456789-6789* is provided.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--related-activity starts-->
	:end-before: <!--related-activity ends-->

| Note: multiple related activities are expressed by repeating the ``related-activity`` element.

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.

2.03
^^^^
Definition of ``related-activity`` element `updated <https://discuss.iatistandard.org/t/hierarchies-related-activity-definition-included-2-03/840>`__.
