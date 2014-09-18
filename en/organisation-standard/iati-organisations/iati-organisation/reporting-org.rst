Example Usage
~~~~~~~~~~~~~
Example ``reporting-org`` for an ``iati-organisation``.
| 
| An example organisation ``ref`` of *AA-AAA-123456789* is declared.
| This example declares an ``OrganisationType`` code *40* (*Multilateral*), using the ``type`` attribute.
| The optional ``secondary-publisher`` boolean is included, for illustration.

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
