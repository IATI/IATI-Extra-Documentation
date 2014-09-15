Example Usage
~~~~~~~~~~~~~
Example usage of ``iati-organisations``.

| This element is a parent for other all other elements of the **IATI Organisation Standard**.

| This example provides a date of *10th September 2014* for the ``generated-datetime`` attribute.
 
| A ``Version`` of *2.01* is declared with the ``version`` attribute.

.. literalinclude:: organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-organisations starts-->
	:end-before: <!--iati-organisation starts-->

The ``iati-organisation`` element acts as a container for other sub-elements.  It is closed as follows:

.. literalinclude:: organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-organisation ends-->	
	:end-before: <!--iati-organisations ends-->
