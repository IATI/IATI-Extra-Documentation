Example Usage
~~~~~~~~~~~~~
Example ``description`` of an ``iati-activity``, with all possible ``DescriptionType`` codes.
Note - it is optional to include all ``DescriptionType``:

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--description starts-->
	:end-before: <!--description ends-->

Additional ``description`` elements can be added for further ``DescriptionType``
It may be appropriate to repeat the ``description`` in other languages using ``xml:lang`` attribute.  
In this example, the language *en* has been set in the ''iati-activity'' element:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--description starts-->
	:end-before: <!--description ends-->
