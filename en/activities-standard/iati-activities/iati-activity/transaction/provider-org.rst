Notes
~~~~~
The unique organisation identifier for the provider organisation. Some
large organisations already have existing codes assigned through the
OECD. For those organisations where no code exists, the organisation can
generate their own code for IATI use in the format of
[country-registration] - [company-registration number]. (e.g. the
organisation identifier for DIPR is: GB-COH-06368740.)

Additional notes
^^^^^^^^^^^^^^^^
Organisation IDs: It is now recommended that organisation ids are built
to a convention, so the schema declaration that @ref must be on a
codelist is out of date. A change to the schema must occur through our
change control process. As such this is flagged for change.

Example Usage
~~~~~~~~~~~~~
The full name of the organisation making the financial ``transaction``
(receiving in the case of loan and interest repayments).:

.. code-block:: xml

        <provider-org>Agency B</provider-org>

The unique Organisation Identifier for the ``provider-org``:

.. code-block:: xml

        <provider-org ref="BB-BBB-123456789-1234AA">Agency B</provider-org>

If the funds are being provided from another reported ``iati-activity``, this
must record the unique ``iati-identifier`` for that ``iati-activity``:

.. code-block:: xml

        <provider-org ref="BB-BBB-123456789" provider-activity-id="BB-BBB-123456789-1234AA" >Agency B</provider-org>
        
Full example:

.. literalinclude:: ../../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--min transaction starts-->
	:end-before: <!--min transaction ends-->
	:emphasize-lines: 6

Full example with additional elements which can override the default value set in ``iati-activity``:  

.. literalinclude:: ../../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--full transaction starts-->
	:end-before: <!--full transaction ends-->
	:emphasize-lines: 6
