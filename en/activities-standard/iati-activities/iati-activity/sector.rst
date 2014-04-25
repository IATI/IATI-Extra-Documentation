Example Usage
~~~~~~~~~~~~~
Example ``sector`` with the ``Sector`` code:

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--sector starts-->
	:end-before: <!--sector ends-->

When multiple ``sector`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``:

.. literalinclude:: ../../activity-standard-example-1.04-annotated-multi.xml
	:language: xml
	:start-after: <!--sector starts-->
	:end-before: <!--sector ends-->
    
The ``vocabulary`` is used to declare which ``sector`` classification list is in use. If this is omitted, then IATI assumes the DAC.

If a vocabulary is not on the ``Vocabulary`` codelist, then the value of *RO* (Reporting Organisation) should be declared:

.. code-block:: xml

    <sector vocabulary="RO">Education</sector>
    
With a text description for the ``Sector``:

.. code-block:: xml

    <sector code="13040">STD control including HIV/AIDS</sector>

Should a description be used that is different to the default language set for the ``iati-activity``, then this can be declared as follows:

.. code-block:: xml

    <sector code="13040" xml:lang="en">STD control including HIV/AIDS</sector>



Changelog
~~~~~~~~~

1.03
^^^^

Where used, the @percentage attribute is now designated as a decimal
value and no longer as a positive Integer
