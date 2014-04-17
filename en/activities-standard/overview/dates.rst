Dates
=====

Definition
----------
Within the **IATI activity standard** several types of dates relating can be specified.

An ``iati-activity`` can have several dates specified.  Those that relate to an ``iati-activity``:

* ``activity-date`` - the planned and actual start and end dates of the activity
* ``transaction-date`` - the date a specific transaction took place
* ``value-date`` - providing the specific date for the value of a ``budget`` or ``transaction``  used for currency conversion purposes
* ``period-start and ``period-end`` dates, used to describe a period of time in a ``budget`` , ``planned-disbursement`` or ``indicator`` 

A time-sensitive declaration, that works in conjunction with the ``activity-date``:

* ``activity-status`` - the stage at which the activity is currently at.

Dates that relate to the publication of the data: 

* ``generated-datetime`` - a date/time stamp for when this *activity-file* was generated. 
* ``last-updated-datetime`` - the last date/time that the data for the specific ''iati-activity`` was updated.

Considerations
--------------

Date format for ``activity-date``, ``period-start``, ``period-end``, ``transaction-date`` and ``value-date`` must be YYYY-MM-DD, eg: 2014-03-21

Date format for ``generated-datetime`` ``last-updated-datetime`` must use ISO 8601 date format, e.g. "2014-03-21T18:45:00+01:00".

A start and end date must be provided - if exact dates are not known then start planned or end planned should be used

Any start date should be before the end date, or the same

All dates can be revised at any point

An ``activity-date`` can have four types:

* start-planned - the forecast start date for the activity (e.g. if your activity is in the pipeline stage or the date of the first disbursement is not known).
* start-actual - the actual start date for the activity (e.g. the date of the first disbursement).
* end-planned - the forecast end date for the activity.
* end-actual - the actual end date for the activity (e.g. the date of the final disbursement).

The ``activity-status`` represents the latest stage for the activity.  It can be updated at any time.

When the ``activity-status`` reaches ``ActivityStatus`` codelist 3, 4 or 5 then it is recommended that an ``end-actual`` date is added

The ``generated-datetime`` is declared at the ``iati-activities`` level.  Is not necessarily the same as the ``last-updated-datetime`` for the individual ``iati-activity`` records within it.

Use of ``generated-datetime`` is highly recommended, to allow recipients to know when a file has been updated.

The ``last-updated-datetime`` date must change whenever the value of any field within the associated ``iati-activity`` changes.

Further guidance
----------------

Reference pages:

* :doc:`activity-date </activities-standard/iati-activities/iati-activity/activity-date/>`
* :doc:`activity-status </activities-standard/iati-activities/iati-activity/activity-status/>`

* :doc:`transaction-date </activities-standard/iati-activities/iati-activity/transaction/transaction-date/>`
* :doc:`budget/period-start </activities-standard/iati-activities/iati-activity/budget/period-start/>`
* :doc:`budget/period-end </activities-standard/iati-activities/iati-activity/budget/period-end/>`

* :doc:`iati-activities </activities-standard/iati-activities/>`
* :doc:`iati-activity </activities-standard/iati-activities/iati-activity/>`

