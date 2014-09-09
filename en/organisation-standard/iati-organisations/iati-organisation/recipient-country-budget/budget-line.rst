Example Usage
~~~~~~~~~~~~~
Example usage of ``budget-line`` in context of ``recipient-country-budget`` element.

| An example ``ref`` attribute is included.

| Multiple budget lines are expressed by repeating the ``budget-line`` element, within the ``recipient-country-budget``.

| In this example, the ``budget-line`` element is only declared within one ``recipient-country-budget``

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-country-budget starts-->
	:end-before: <!--recipient-country-budget ends-->
	:emphasize-lines: 8, 11, 12, 15
			
Changelog
~~~~~~~~~

2.01
^^^^

| The ``budget-line`` element was introduced in 2.01.

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of integers.
