Example Usage
~~~~~~~~~~~~~
Example of ``reference`` in the context of a ``result`` element.

| This example declares use of ``@vocabulary`` *99*, with a ``@code`` of *B1*.  The ``@vocabulary-uri`` attribute should also be used:

.. code-block:: xml

    <reference vocabulary="99" code="B1" vocabulary-uri="http://example.com/indicators.html" />

| The ``reference`` element can be repeated in any ``result``. If the ``reference`` element is reported at result level it must not be reported at indicator level:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result-reference starts-->
	:end-before: <!--result-reference ends-->

Changelog
~~~~~~~~~

2.03
^^^^
The optional ``reference`` element was `added <https://discuss.iatistandard.org/t/results-vocabulary-attribute-option-included-2-03/879>`__.
