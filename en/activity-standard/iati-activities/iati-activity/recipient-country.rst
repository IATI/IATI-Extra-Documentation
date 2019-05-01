Example Usage
~~~~~~~~~~~~~
Example ``recipient-country`` of an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*AF*) from the *Country* codelist.

.. code-block:: xml

        <recipient-country code="AF" />

| The ``recipient-country`` element can be repeated in any ``iati-activity``.
| When multiple ``recipient-country`` are declared, then the ``@percentage`` values should sum to 100% for the specific ``iati-activity``:

.. code-block:: xml

	<recipient-country code="AF" percentage="50" />
	<recipient-country code="AG" percentage="50" />

| When both the ``recipient-region`` and ``recipient-country``, then the ``@percentage`` values should sum to 100% per region vocabulary for the specific ``iati-activity``.

.. code-block:: xml

	<recipient-country code="AF" percentage="50" />
	<recipient-region code="489" vocabulary="1" percentage="50" /> 

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is no longer allowed with this element.  It should `now be declared <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#narrative-new-elements>`__  with the new child ``narrative`` element, but only in particular use-cases.

1.03
^^^^
Where used, the ``@percentage`` attribute is now designated as a decimal value and no longer as a positive Integer
