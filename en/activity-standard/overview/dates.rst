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
	* start-planned - the forecast start date for the ``iati-activity`` (e.g. if the ``iati-activity`` is in the pipeline stage or the date of the first disbursement is not known).
	* start-actual - the actual start date for the ``iati-activity`` (e.g. the date of the first disbursement).
	* end-planned - the forecast end date for the ``iati-activity``.
	* end-actual - the actual end date for the ``iati-activity`` (e.g. the date of the final disbursement).
* The ``activity-status`` represents the latest stage for the activity.  It can be updated at any time.
* When the ``activity-status`` reaches ``ActivityStatus`` codes *3*, *4* or *5* then it is recommended that an ``end-actual`` date is added.
* ``ActivityStatus`` code *6* indicates a temporary suspension of an activity. In this state an activity is assumed not to be ``current``, but future, forward-looking budgets are still assumed to be applicable.

