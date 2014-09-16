Example Usage
~~~~~~~~~~~~~
| Example of ``recipient-country-budget`` for a single ``recipient-country`` *AF*.

| Periods are stated using ``period-start`` and ``period-end``, with dates in ISO 8601 format (YYYY-MM-DD).

| The ``value`` example includes a ``currency`` of *USD* - which differs from that set as ``default-currency`` in ``iati-organisation``.

| The ``value-date`` is reported in ISO 8601 format (YYYY-MM-DD).

| Note: multiple budgets are expressed by repeating the ``recipient-country-budget`` element.
| This example ``recipient-country-budget`` is reported for years *2014, *2015* and *2016*.
		
.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-country-budget starts-->
	:end-before: <!--recipient-country-budget ends-->
	:emphasize-lines: 1, 16, 17, 22, 23, 28
