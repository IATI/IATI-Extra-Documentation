Example Usage
~~~~~~~~~~~~~
Example usage of ``aid-type`` of a ``transaction`` in an ``iati-activity``.

| The ``@code`` attribute declares a valid code from the specified codelist.
| The ``@vocabulary`` attribute declares a valid code (*1*) from the *AidTypeVocabulary* codelist.

.. code-block:: xml

	<aid-type code="A01" vocabulary="1" />
	
The aid-type element can be repeated in any iati-activity.

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->

The vocabulary is used to declare which AidType list is in use. If omitted, an AidType Vocabulary of 1 (OECD DAC) is assumed.

| Note: The ``aid-type`` element can override the ``default-aid-type`` value set in ``iati-activity``

Changelog
~~~~~~~~~

2.03
^^^^
The ``aid-type`` element can be reported multiple times within a ``transaction`` element `added <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__.
The ``@code`` attribute definition was `updated <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__.
The ``@vocabulary`` attribute was `added <https://discuss.iatistandard.org/t/add-vocabularies-to-aid-type-included-2-03/847>`__.
