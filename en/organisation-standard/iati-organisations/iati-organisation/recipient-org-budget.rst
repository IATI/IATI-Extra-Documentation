Example Usage
~~~~~~~~~~~~~
Example of ``recipient-org-budget`` for a single ``recipient-org`` *123*.
Periods are stated using ``period-start`` and ``period-end``, with dates in ISO 8601 format (YYYY-MM-DD).
This example ``recipient-org-budget`` is reported for years *2014, *2015* and *2016*.
The ``value`` example includes a ``currency`` of *USD* - which differs from that set as ``default-currency`` in ``iati-organisation``.
The ``value-date`` is reported in ISO 8601 format (YYYY-MM-DD).
		
.. literalinclude:: ../../organisation-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--recipient-org-budget starts-->
	:end-before: <!--recipient-org-budget ends-->
	:emphasize-lines: 1, 6, 7, 12, 13, 18
