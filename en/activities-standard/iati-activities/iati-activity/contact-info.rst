Example Usage
~~~~~~~~~~~~~

This element is a container for other sub elements:

.. code-block:: xml

        <contact-info type="1">
           ....
        </contact-info>

Example containing all possible child elements: ``organisation``;``person-name``;``job-title``;``mailing-address``; ``telephone``; ``email``; ``website``.

.. code-block:: xml

    <contact-info type="1">
      <organisation>Agency A</organisation>
      <person-name>A. Example</person-name>
      <job-title>Transparency Lead</job-title>
      <mailing-address>Transparency House, The Street, Town, City, Postcode</mailing-address>
      <telephone>0044111222333444</telephone>
      <email>transparency@example.org</email>
      <website>http://www.example.org</website>
    </contact-info>

Changelog
~~~~~~~~~

1.03
^^^^

Added the optional contact-info/website element

Added the optional contact-info/@type attribute

Changed the following subelements of contact-info to allow multiple-language versions explicitly (no change to parsing; purely
semantic):

-  organisation
-  person-name
-  job-title
-  mailing-address
