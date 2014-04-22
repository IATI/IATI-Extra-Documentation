Example Usage
~~~~~~~~~~~~~
Example ``recipient-country`` with relevant ``Country`` code:

.. code-block:: xml

    <recipient-country code="CG"/>

Additionally, the name of the ``Country`` can also be declared:

.. code-block:: xml

    <recipient-country code="CG">Democratic Republic of Congo</recipient-country>

When multiple ``recipient-country`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``:

.. code-block:: xml

    <recipient-country code="CG" percentage="60"/>
    <recipient-country code="AO" percentage="40"/>
    

Changelog
~~~~~~~~~

1.03
^^^^

Where used, the ``percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
