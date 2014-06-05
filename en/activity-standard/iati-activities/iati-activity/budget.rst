Example Usage
~~~~~~~~~~~~~
The ``budget`` element acts as a container for other sub elements.

The attribute ``type`` should declare the relevant ``BudgetType`` code.  
If omitted, then ``BudgetType`` *Original* (code 1) is assumed:

Example ``budget`` for a single year:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--budget starts-->
	:end-before: <!--budget ends-->
	:emphasize-lines: 1, 5

Example ``budget`` over multiple years:

.. literalinclude:: ../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--budget starts-->
	:end-before: <!--budget ends-->
	:emphasize-lines: 1, 5, 6, 10, 11, 15, 16, 20
