Example Usage
~~~~~~~~~~~~~
Example ``default-aid-type``  for an ``iati-activity``.

| The ``@code`` attribute declares a valid code from the specified codelist.
| The ``@vocabulary`` attribute declares a valid code (*1*) from the *AidTypeVocabulary* codelist.

.. code-block:: xml

	<default-aid-type code="A01" vocabulary="1" />


The default-aid-type element can be repeated in any iati-activity.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--default-aid-type starts-->
	:end-before: <!--default-aid-type ends-->

The vocabulary is used to declare which AidType list is in use. If omitted, an AidType Vocabulary of 1 (OECD DAC) is assumed. 

| Note: The ``aid-type`` element can override the ``default-aid-type`` value set in ``iati-activity``

Changelog
~~~~~~~~~
2.03
^^^^
The ``default-aid-type`` element can be reported multiple times within a ``iati-activity`` element `added <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__.
The ``@code`` attribute definition was `updated <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__.
The ``@vocabulary`` attribute was `added <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__.

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.
