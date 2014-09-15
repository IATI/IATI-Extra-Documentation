Example Usage
~~~~~~~~~~~~~
Example usage of  `iati-organisation``

| This example provides a date of *10th September 2014* for the ``last updated-datetime`` attribute.

| This element is a parent for other child elements.

| This example declares a ``Language`` as *en* (*English*) with the ``xml:lang`` attribute.

| A ``Currency`` of *EUR* (*Euros*) is set with the ``default-currency`` attribute.  

.. literalinclude:: ../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-organisation starts-->
	:end-before: <!--organisation-identifier starts-->

The ``iati-organisation`` element acts as a container for other sub-elements.  It is closed as follows:

.. literalinclude:: ../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--multi-country-document-link ends-->	
	:end-before: <!--iati-organisation ends-->
