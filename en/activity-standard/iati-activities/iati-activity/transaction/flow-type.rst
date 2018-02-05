Example Usage
~~~~~~~~~~~~~
Example usage of ``flow-type`` of a ``transaction`` in an ``iati-activity``.

| The ``@code`` attribute declares a valid code (*20*) from the *FlowType* codelist.

| Note: The ``flow-type`` element can override the ``default-flow-type`` value set in ``iati-activity``:

.. literalinclude:: ../../../activity-standard-example-annotated.xml
	:language: xml
	:start-after: <!--transaction starts-->
	:end-before: <!--transaction ends-->

Changelog
~~~~~~~~~

2.01
^^^^
Freetext is `no longer allowed <http://iatistandard.org/upgrades/integer-upgrade-to-2-01/2-01-changes/#freetext-amended-elements>`__  within this element.
