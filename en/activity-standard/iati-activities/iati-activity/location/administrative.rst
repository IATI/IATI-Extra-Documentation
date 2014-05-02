Example Usage
~~~~~~~~~~~~~
Example usage of ``administrative`` within context of ``location``:

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--location starts-->
	:end-before: <!--location ends-->
	:emphasize-lines: 7

Prior to 1.04 National and sub-national administrative divisions could be declared as
such (but as of 1.04 the @country, @adm1 and @adm2 attributes are deprecated):

.. code-block:: xml

    <administrative country="AF" adm1="KAN">Kandahar Province, Afghanistan</administrative>

Changelog
~~~~~~~~~

1.04
^^^^

| In 1.04 the @country, @adm1 and @adm2 attributes were deprecated. The new attributes replace the function of the previous ones.
