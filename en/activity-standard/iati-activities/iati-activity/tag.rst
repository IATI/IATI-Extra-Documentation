Example Usage
~~~~~~~~~~~~~
Example ``tag`` in a ``iati-activity`` element.

| The ``@vocabulary`` attribute declares a valid code (*1*) from the *TagVocabulary* codelist.
| An example value *1* from this vocabulary is declared with the ``@code`` attribute.

.. code-block:: xml

	<tag vocabulary="1" code="1" />

| The ``tag`` element can be repeated in any ``iati-activity``.

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--tag starts-->
	:end-before: <!--tag ends-->

| If a vocabulary is not on the *TagVocabulary* codelist, then the value of *99* (Reporting Organisation) should be declared.

| If a publisher uses a vocabulary of 99 (i.e. 'Reporting Organisation'), then the ``@vocabulary-uri`` attribute should also be used, for example:

.. code-block:: xml

    <tag vocabulary="99" vocabulary-uri="http://example.com/vocab.html" code="T1" />


Changelog
~~~~~~~~~

2.03
^^^^
The ``tag`` element within a ``iati-activity`` element was `added <https://discuss.iatistandard.org/t/non-statistical-secondary-sectors-excluded-2-03/849>`__.
