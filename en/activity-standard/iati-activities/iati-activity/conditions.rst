Example Usage
~~~~~~~~~~~~~
Example ``conditions`` for an ``iati-activity``.

| This element is a parent for ``condition`` child element(s).

| The ``@attached`` *0* boolean is included, for illustration of no conditions.

.. code-block:: xml

     <conditions attached="0"/>

| The ``@attached`` *1* boolean is included, for illustration of conditions.

.. code-block:: xml

     <conditions attached="1">
     ...
     </conditions>

| Full example with all child elements:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--conditions starts-->
	:end-before: <!--conditions ends-->

