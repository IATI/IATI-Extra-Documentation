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
The ``sector`` element was `added <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#transaction-new-child-elements>`__ as a child element of ``transaction``.
