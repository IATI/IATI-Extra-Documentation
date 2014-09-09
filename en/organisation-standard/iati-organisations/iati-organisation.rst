Example Usage
~~~~~~~~~~~~~
Example of ``iati-organisation`` with ``last updated-datetime`` of on 9th September 2014. 
Language set as *en* (English) and a ``default-currency`` to *EUR* (Euros).  
The optional ``version`` of *2.01* is also stated:

.. literalinclude:: ../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--iati-organisation starts-->
	:end-before: <!--organisation-identifier starts-->

The ``iati-organisation`` element acts as a container for other sub-elements.  It is closed as follows:

.. literalinclude:: ../organisation-standard-example-annotated.xml
	:language: xml
	:start-after: <!--multi-country-document-link ends-->	
	:end-before: <!--iati-organisation ends-->
