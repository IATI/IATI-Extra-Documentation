Example Usage
~~~~~~~~~~~~~
Example title for an ``iati-activity``:

.. literalinclude:: ../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--title starts-->
	:end-before: <!--title ends-->

If a default langage has not been declared in the ``iati-activity`` element, then a language should be specified

.. code-block:: xml

        <title xml:lang="en">Activity title</title>

It may be appropriate to repeat the ``title`` in other languages using ``xml:lang`` attribute.  In this example, the language *en* has been set in the ''iati-activity'' elenment:

.. literalinclude:: ../../activity-standard-example-annotated-multi.xml
	:language: xml
	:start-after: <!--title starts-->
	:end-before: <!--title ends-->
	  
Note: It is recommended to provide a ``title`` in the language(s) spoken in the country(ies) where the ``iati-activity`` take place, or is aimed at.
