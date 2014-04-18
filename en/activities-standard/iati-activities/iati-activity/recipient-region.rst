Example Usage
~~~~~~~~~~~~~
Example ``recipient-region`` with relevant ``Region`` code:

.. code-block:: xml

    <recipient-region code="289"/>

Additionally, the name of the ``Region`` can also be declared.

.. code-block:: xml

    <recipient-region code="289">South of Sahara, regional<recipient-region>

When multiple ``recipient-region`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``:

.. code-block:: xml

    <recipient-region percentage="60" code="289">South of Sahara, regional</recipient-region>
    <recipient-region percentage="40" code="189">North of Sahara, regional</recipient-region>
    

Additionally, a ``RegionVocabulary`` can also be declared in this element:

.. code-block:: xml

    <recipient-region vocabulary="1" code="289">South of Sahara, regional</recipient-region>

Changelog
~~~~~~~~~

1.03
^^^^

Where used, the ``percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
