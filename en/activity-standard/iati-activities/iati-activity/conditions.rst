Example Usage
~~~~~~~~~~~~~
The ``conditions`` element acts as a container for other sub elements. 
| 
| Example of no ``conditions`` attached to the ``iati-activity`` :

.. code-block:: xml

     <conditions attached="0"/>

Example of ``conditions`` attached to the ``iati-activity``, expressed through the bolean *1*:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--conditions starts-->
	:end-before: <!--conditions ends-->
	:emphasize-lines: 1, 3

From version 1.04, the schema allows the ``xml:lang`` attribute to also be included in the sub-element ``condition``
|
| Example of an ``iati-activity`` with two ``conditions``, declared in the default language of *en*,  and also *fr*:

.. literalinclude:: ../../activity-standard-example-annotated-multi.xml	
	:language: xml
	:start-after: <!--conditions starts-->
	:end-before: <!--conditions ends-->
	:emphasize-lines: 1, 6
