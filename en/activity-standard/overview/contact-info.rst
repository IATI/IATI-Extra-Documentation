Contact Info
============

Definition
----------
The **IATI activity standard** enables ``contact-info`` to be included for any ``iati-activity``

The following fields can be included:

* ``organisation``
* ``person-name``
* ``job-title``
* ``telephone``
* ``email``
* ``mailing-address``
* ``website``


Considerations
--------------
When using the **IATI activity standard** to declare *contact info*, the following should be considered:

* Any ``contact-info`` should include at least one of the available fields.
* More than one ``contact-info`` can be included within an ``iati-activity``.
* Use of the *ContactType* code is recommended, especially when declaring multiple ``contact-info``.
* Careful attention should be paid to personal data being published.  Always include organisational ``contact-info``.
* Telephone numbers should include the international dialing code.  Avoid presentation of internal ``telephone`` numbers.
* The free-text instances of ``organisation``, ``person-name``, ``job-title`` and ``mailing-address`` should avoid use of text in CAPITALS, where possible. 


2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* Any freetext text for ``organisation``, ``person-name``, ``job-title`` and ``mailing-address`` must be included in a child ``narrative`` element, which can be repeated for different languages.
