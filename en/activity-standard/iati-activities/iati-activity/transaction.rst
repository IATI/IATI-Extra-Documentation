Example Usage
~~~~~~~~~~~~~
Example ``transaction`` in an ``iati-activity``.

| This element is a parent for other child elements.

| An example ``@ref`` of *1234* is declared.

.. code-block:: xml

        <transaction ref="1234">
        ....
        </transaction>

| An example which would denote this as a humanitarian transaction i.e. with the ``@humanitarian`` element set to '1'.

.. code-block:: xml

        <transaction ref="1234">
        ....
        </transaction>

| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->
	:emphasize-lines: 1, 23
	    
| The ``transaction`` element can be repeated in any ``iati-activity``.  


Changelog
~~~~~~~~~

2.02
^^^^
| The ``humanitarian`` attribute was `added <http://support.iatistandard.org/entries/106937796-Humanitarian-Flag>`__.    
