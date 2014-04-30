Example Usage
~~~~~~~~~~~~~
The ``budget`` element acts as a container for other sub elements.

The attribute ``type`` should declare the relevant ``BudgetType`` code.  
If omitted, then ``BudgetType`` *Original* (code 1) is assumed:

Example ``budget`` for a single year:

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--budget starts-->
	:end-before: <!--budget ends-->

Example ``budget`` over multiple years:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--budget starts-->
	:end-before: <!--budget ends-->
