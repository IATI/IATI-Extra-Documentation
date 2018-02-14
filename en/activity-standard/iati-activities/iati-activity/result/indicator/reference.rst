Example Usage
~~~~~~~~~~~~~
Example of ``reference`` in the context of an ``indicator`` of a ``result`` element.

| This example declares use of ``@vocabulary`` *1*, with a ``@code`` of *3429*:

.. code-block:: xml

    <reference vocabulary="1" code="3429" />


If a publisher uses a vocabulary of 99 (i.e. 'Reporting Organisation'), then the ``@indicator-uri`` attribute should also be used, for example:

.. code-block:: xml

	<reference vocabulary="99" code="B1" indicator-uri="http://example.com/indicators.html" />


| The ``reference`` element can be repeated in any ``indicator``.  If the ``reference`` element is reported at indicator level it must not be reported at result level:

.. literalinclude:: ../../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--result starts-->
	:end-before: <!--result ends-->

Changelog
~~~~~~~~~

2.03
^^^^
Definition of ``@indicator-uri`` attribute `updated <https://discuss.iatistandard.org/t/guidance-on-u-r-i-usage-for-publisher-s-own-vocabularies-included-2-03/850>`__.

The rule for using the ``reference`` element was `added <https://discuss.iatistandard.org/t/results-vocabulary-attribute-option-included-2-03/879>`__.

2.02
^^^^
The optional ``reference`` element was `added <http://support.iatistandard.org/entries/79784435-Results-Require-unambiguous-indicator-reference>`__.
