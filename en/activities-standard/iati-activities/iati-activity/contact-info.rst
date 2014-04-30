Example Usage
~~~~~~~~~~~~~
This element acts as a container for other sub elements.

Example ``contact-info`` that declares ``ContactType`` code *1*:

.. code-block:: xml

        <contact-info type="1">
           ....
        </contact-info>

Example ``contact-info`` containing all possible child elements: ``organisation`` ; ``person-name`` ; ``job-title`` ; ``mailing-address`` ; ``telephone`` ; ``email`` ; ``website``

.. literalinclude:: ../../activity-standard-example-1.04-annotated.xml
	:language: xml
	:start-after: <!--contact-info starts-->
	:end-before: <!--contact-info ends-->
	:emphasize-lines: 1, 9

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
