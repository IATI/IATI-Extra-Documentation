Self-defined Vocabularies
=========================



Definition
----------
For several elements in the **IATI activity standard** and the **IATI organisation standard**, the *vocabulary* for a given code can be set via the ``@vocabulary`` attribute:

A good example of this is the ``sector`` element, which will typically be given a 5-digit ``code`` such as "11120". However, this code only makes sense to data users if they know which sector codelist it is from.

To achieve this, the ``sector``/``@vocabulary`` should be set to the appropriate entry on the `SectorVocabulary <http://iatistandard.org/codelists/SectorVocabulary/>`__ codelist. For "11120", this would be vocabulary ``"1"`` - the *OECD DAC CRS Purpose Codes (5 digit)*, and would hence denote the code for `Education facilities and training <http://iatistandard.org/201/codelists/Sector/>`__.

It's important to note that if there are multiple sectors given from the same vocabulary, their ``@percentage`` attributes should add up to 100.

Here is an example:

.. code-block:: xml

    <iati-activity>
        <!-- Other elements -->
        <sector vocabulary="1" code="11120" percentage="50" />
        <sector vocabulary="1" code="11121" percentage="50" />
        <!-- Other elements -->
    </iati-activity>

For any given element that has a ``@vocabulary`` attribute, the guidance on this site will link to the relevant codelist, which can be seen in the guidance for the `sector <http://iatistandard.org/activity-standard/iati-activities/iati-activity/sector/#sector>`__ element.

For each of these vocabularies, there is almost always the option for a publisher to provide their own. For instance, if a publisher wants to declare that an activity is "11120" for the OECD DAC 5-digit vocabulary, but also wants to declare it as "general_education" on their own codelist, they would simply have to set the vocabulary to "Reporting Organisation" (which is usually **but not always** ``"99"``), and then use the ``@vocabulary-uri`` attribute to link through to their own (machine-readable) codelist.

Here is an example:

.. code-block:: xml

    <iati-activity>
        <!-- Other elements -->
        <sector vocabulary="99" vocabulary-uri="http://example.com/vocab.html" code="general_education" percentage="100" />
        <!-- Other elements -->
    </iati-activity>

Considerations
--------------
When using the **IATI activity standard** to declare *budgets*, the following should be considered:

* It is very important that ``@percentages`` add up to 100 per vocabulary.
* When a publisher uses code ``"99"``, or whichever other code denotes that they are using a *Reporting Organisation* provided codelist, they should provide the corresponding ``@vocabulary-uri`` (or equivalent) attribute.

Pre 2.02 Considerations
-----------------------

Not all of the elements mentioned above exist in some previous versions of the standard, but most of them do in version 2.01, and this practice should be standard in all 2.xx versions and above.
