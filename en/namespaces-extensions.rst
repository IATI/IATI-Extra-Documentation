Namespaces & Extensions
=======================

Adding other information
------------------------

There will be situations where reporting organisations want to publish additional data that are not covered by the default IATI elements, or want to specify the data using the original formats or values to avoid information loss.  IATI provides two mechanisms for doing so:

* Use an XML namespace to extend the schema.
* Use the legacy-data element to provide original data values.


XML namespaces
--------------

The first approach allows reporting organisations to invent any required markup and add it to an IATI activity report.  IATI users who don’t recognise the extended markup are required simply to ignore it, without reporting an error.  Here is an example:

.. code-block:: xml

    <iati-activity xmlns:acme="http://example.org/acme/ns#">

    ...

    <acme:risk-level>3</acme:risk-level>

    ...

    </iati-activity>

In this example, ACME has defined its own namespace using the URL ``http://example.org/acme/ns#`` and mapped that to the prefix ``acme``.  It then adds the new element, ``acme:risk-level``, to provide information about its risk assessment for the activity.  IATI users who don’t recognise the ``http://example.org/acme/ns#`` namespace are required to ignore the ``acme:risk element`` rather than reporting an error, so the extended markup does not harm compatibility.  Users who are familiar with the namespace, however, can take advantage of the additional information.

