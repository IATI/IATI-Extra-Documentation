Example Usage
~~~~~~~~~~~~~

The Indicator element is contained within a result set, and also
contains other elements.

The type of measurement for the indicator value described.:

.. code-block:: xml

    <result>
    ....
        <indicator measure="1">
        ....
        </indicator>
    .....
    </result>    

Additionally, a flag to indicate whether the data in this indicator
improves from small to large (ascending = “1”), or whether it is
reversed and improves from large to small (ascending=“0”). Boolean.
If omitted, then '1' is assumed.

.. code-block:: xml

    <result>
    ....
        <indicator measure="1" ascending="1">
        ....
        </indicator>
    .....
    </result>    
