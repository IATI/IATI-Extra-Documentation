Example Usage
~~~~~~~~~~~~~
Example ``budget-line`` for ``total-budget`` of an ``iati-orgaisation``.

| An example ``ref`` attribute is included.

.. code-block:: xml
	:emphasize-lines: 1, 4
	
		<budget-line ref="1234">
			<value value-date="2014-01-01">200000000</value>
			<narrative>Budget Line 1</narrative>
		</budget-line>

| The ``budget-line`` element can be repeated in any ``total-budget``. 
| In this example, the ``budget-line`` element is only declared within one ``total-budget``

.. literalinclude:: ../../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--total-budget starts-->
	:end-before: <!--total-budget ends-->
	:emphasize-lines: 5, 8, 9, 12
			
Changelog
~~~~~~~~~

2.01
^^^^

| The ``budget-line`` element was introduced in 2.01.

1.03
^^^^

Currency values are now allowed to be declared as decimals instead of integers.
