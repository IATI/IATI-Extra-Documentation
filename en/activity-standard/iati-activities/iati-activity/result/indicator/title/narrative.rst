Example Usage
~~~~~~~~~~~~~
The ``narrative`` child element can be used to declare freetext for the ``title`` parent element.

.. code-block:: xml

		<title>
			<narrative>Indicator title</narrative>
			<narrative xml:lang="fr">Indicator titre</narrative>
		</title>

The ``narrative`` element can be repeated for any language additional to the default language set in ``iati-activity``, by using the ``@xml:lang`` attribute:

.. code-block:: xml

		<title>
			<narrative>Indicator title</narrative>
			<narrative xml:lang="fr">Indicator titre</narrative>
		</title>

Changelog
~~~~~~~~~

2.01
^^^^

| The ``narrative`` element was introduced in 2.01.
