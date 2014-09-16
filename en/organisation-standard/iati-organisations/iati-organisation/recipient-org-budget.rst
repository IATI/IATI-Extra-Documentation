Example Usage
~~~~~~~~~~~~~
| Example of ``recipient-org-budget`` for a single ``recipient-org`` *123*.

| Periods are stated using ``period-start`` and ``period-end``, with dates in ISO 8601 format (YYYY-MM-DD).

| The ``value`` example includes a ``currency`` of *USD* - which differs from that set as ``default-currency`` in ``iati-organisation``.

| The ``value-date`` is reported in ISO 8601 format (YYYY-MM-DD).

| Note: multiple budgets are expressed by repeating the ``recipient-org-budget`` element.
| This example ``recipient-org-budget`` is reported for years *2014, *2015* and *2016*.

		
.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--recipient-org-budget starts-->
	:end-before: <!--recipient-org-budget ends-->
	:emphasize-lines: 1, 16, 17, 24, 25, 32
