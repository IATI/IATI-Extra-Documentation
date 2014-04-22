Example Usage
~~~~~~~~~~~~~
This is a child element of ``country-budget-items``

Example that declares ``BudgetIdentifier`` code *1.1.1* (Executive - executive) with a ``percentage`` of *80*
.. code-block:: xml

      <budget-item code="1.1.1" percentage="80">
         <description xml:lang="en">XXX</description>
      </budget-item>

When multiple ``budget-item`` are declared, then the ``percentage`` values should sum to 100% for the specific ``iati-activity``:

.. code-block:: xml

    <country-budget-items vocabulary="2">
      <budget-item code="1.1.1" percentage="80">
        <description>Description text</description>
      </budget-item>
    </country-budget-items>
    <country-budget-items vocabulary="2">
      <budget-item code="1.1.2" percentage="20">
        <description>Description text</description>
      </budget-item>
    </country-budget-items>

Full example:

.. code-block:: xml

    <country-budget-items vocabulary="2">
      <budget-item code="1.1.1"/>
        <description>Description text</description>
      </budget-item>
    </country-budget-items>

Changelog
~~~~~~~~~

1.03
^^^^

Added the optional country-budget-item element

1.02
^^^^

This element did not exist

1.01
^^^^

This element did not exist
