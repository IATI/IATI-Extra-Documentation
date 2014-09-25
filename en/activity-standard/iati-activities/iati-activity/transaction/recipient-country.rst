Example Usage
~~~~~~~~~~~~~
Example ``recipient-country`` of ``transaction`` in an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*AF*) from the *Country* codelist.

.. code-block:: xml

        <recipient-country code="AF" />

Full example:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 17
 

Changelog
~~~~~~~~~

2.01
^^^^
The ``recipient-country`` element was added to ``transaction`` in 2.01
