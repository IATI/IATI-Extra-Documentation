Example Usage
~~~~~~~~~~~~~
Example usage of ``period-start`` in context of ``planned-disbursement`` element.

A date in ISO 8601 format (YYYY-MM-DD) for the ``period-start`` date of the reporting period is required:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->
	:emphasize-lines: 2

Example that declares multiple ``planned-disbursements. 

Note - in this example, only the ``period-start`` date element is present, to declare the disbursement is flagged for a specific date, rather than a period of time.

In this example, optional text has also been included, to provide further clarification:

.. literalinclude:: ../../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--planned-disbursement starts-->
	:end-before: <!--planned-disbursement ends-->
	:emphasize-lines: 2, 6, 10
