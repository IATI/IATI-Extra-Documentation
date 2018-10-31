Activity Dates
==============

Definition
----------
Within the **IATI activity standard** several types of dates can be specified.

Dates that relate directly to the ``iati-activity``:

* ``activity-date`` - the planned and actual start/end dates of the ``iati-activity``.
* ``transaction-date`` - the date a specific ``transaction`` took place.
* ``value-date`` - the specific date for the ``value`` of a ``budget`` or ``transaction``, which is used for currency conversion purposes.
* ``period-start`` and ``period-end`` dates are used to describe a period of time in a ``budget`` , ``planned-disbursement`` or ``indicator`` 

| Additionally, a time-sensitive (non-date) declaration works in conjunction with the ``activity-date``:

* ``activity-status`` - a numeric code to declare current stage of the ``iati-activity``.


Considerations
--------------
When using the **IATI activity standard** to declare *dates*, the following should be considered:

* Date format for ``activity-date``, ``period-start``, ``period-end``, ``transaction-date`` and ``value-date`` must be in ISO 8601 (YYYY-MM-DD), eg: 2014-03-21
* Date format for ``generated-datetime`` ``last-updated-datetime`` must use ISO 8601 date format, e.g. "2014-03-21T18:45:00+01:00".
* A start and end date must be provided - if exact dates are not known then start planned or end planned should be used
* Any start date should be before the end date, or the same
* All dates can be updated at any point
* An ``activity-date`` can have four types:
	* start-planned (code *1*) - the forecast start date for the ``iati-activity`` (e.g. if the ``iati-activity`` is in the pipeline stage or the date of the first disbursement is not known).
	* start-actual (code *2*) - the actual start date for the ``iati-activity`` (e.g. the date of the first disbursement).
	* end-planned (code *3*) - the forecast end date for the ``iati-activity``.
	* end-actual (code *4*)- the actual end date for the ``iati-activity`` (End dates should, wherever possible, reflect the ending of physical activity.).
* The ``activity-status`` represents the latest stage for the activity.  It can be updated at any time.
* When the ``activity-status`` reaches *ActivityStatus* codes *3*, *4* or *5* then it is recommended that an end-actual (code *4*) date is added.

2.01+ Considerations
--------------------
In versions 2.01 and above, the following must also be considered:

* The *ActivityDateType* codes for ``activity-date`` have changed to being numeric in versions 2.01 and above.
* Dates must be a valid *xsd:date*, and a datetimes must be a valid *xsd:dateTime*.
