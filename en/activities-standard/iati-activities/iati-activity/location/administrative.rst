

Example Usage
~~~~~~~~~~~~~

.. code-block:: xml

    <administrative code="" vocabulary="" level="">Administrative information here</administrative>

Prior to 1.04 National and sub-national administrative divisions could be declared as
such (but as of 1.04 the @country, @adm1 and @adm2 attributes are deprecated:

.. code-block:: xml

    <administrative country="AF" adm1="KAN">Kandahar Province, Afghanistan</administrative>

Changelog
~~~~~~~~~

1.04
^^^^

| In 1.04 the @country, @adm1 and @adm2 attributes were deprecated. The new attributes replace the function of the previous ones.
