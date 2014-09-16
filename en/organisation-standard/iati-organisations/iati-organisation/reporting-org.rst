Example Usage
~~~~~~~~~~~~~
Example ``reporting-org`` for an ``iati-organisation``.

| The organisation ``ref`` of *AA-AAA-123456789* is declared.

| An ``OrganisationType`` code of *40* (*Multilateral*) is used.

| The optional ``secondary-publisher`` boolean is included, for illustration:

.. literalinclude:: ../../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--reporting-org starts-->
	:end-before: <!--reporting-org ends-->
	:emphasize-lines: 1, 4	
	
		
Changelog
~~~~~~~~~

1.04
^^^^

| The ``secondary-publisher`` attribute was introduced in 1.04.
