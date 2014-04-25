Example Usage
~~~~~~~~~~~~~
Example of ``total-budget`` for a single ``iati-organisation``.
Periods are stated using ``period-start`` and ``period-end``, with dates in ISO 8601 format (YYYY-MM-DD).
This example ``total-budget`` is reported for years *2014, *2015* and *2016*.
The ``value`` example includes a ``currency`` of *USD* - which differs from that set as ``default-currency`` in ``iati-organisation``.
The ``value-date`` is reported in ISO 8601 format (YYYY-MM-DD).
		
.. literalinclude:: ../../organisation-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--total-budget starts-->
	:end-before: <!--total-budget ends-->
