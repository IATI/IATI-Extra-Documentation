Example Usage
~~~~~~~~~~~~~
Example ``conditions`` for an ``iati-activity``.

| This element is a parent for ``condition`` child element(s).
 
| Example of no ``conditions`` attached to the ``iati-activity``, expressed through the bolean *0*:

.. code-block:: xml

     <conditions attached="0"/>

| Example of ``conditions`` attached to the ``iati-activity``, expressed through the bolean *1*:

.. code-block:: xml

     <conditions attached="1">
     ...
     </conditions>
     
| Full example with all child elements:     
     
.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--conditions starts-->
	:end-before: <!--conditions ends-->
	:emphasize-lines: 1, 6
