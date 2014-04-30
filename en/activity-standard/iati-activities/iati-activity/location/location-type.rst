

Example Usage
~~~~~~~~~~~~~

Just the code can be declared

.. code-block:: xml

    <location-type code="PPL"/>

Additionally the description for this code can be stated

.. code-block:: xml

    <location-type code="PPL">populated place</location-type>

Where the description is in a language other than the activity default,
then this should be declared:

.. code-block:: xml

    <location-type code="PPL" xml:lang-"fr">region peuplee</location-type>

Changelog
~~~~~~~~~

1.04
^^^^

| Deprecated in 1.04
| The location-type element was deprecated in 1.04. The location-class element should be used instead.
