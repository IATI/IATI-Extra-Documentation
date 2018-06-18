Country Budget Alignment
========================

Guidance on implementing budget and aid alignment
-------------------------------------------------
During the 2.03 upgrade process, decision was made to deprecate BudgetIdentifier codelist. As a result, further guidance was required to provide to publishers on implementing aid and budget alignment.
This guidance explains how the methodology now works. It stems from work conducted by the IATI TAG 2017 Working Group on Aid and Budget Alignment, and reflects decisions made by the WP-STAT and IATI Steering Committee. In summary:

1) Publish the capital-spend field
----------------------------------
For activities at the commitment stage, the percentage of an activity that is capital expenditure should be published using the ``capital-spend`` field. The definition of capital expenditure follows the IMF GFS definition:

  Capital spending is generally defined as physical assets with a useful life of more than one year. But it also includes capital improvements or the rehabilitation of physical assets that enhance or extend the useful life of the asset (as distinct from repair or maintenance, which assures that the asset is functional for its planned life). Capital includes all aspects of design and construction that are required to make the asset operational. Source: D Jacobs, 2009, Capital Expenditures and the Budget, IMF PFM Technical Guidance Note No 8. (IMF, Washington)]

This definition was approved by `WP-STAT under the written procedure <http://www.oecd.org/officialdocuments/publicdisplaydocumentpdf/?cote=DCD/DAC/STAT(2015)30/REV1&docLanguage=En/>`_ in February 2016.


2) Publish detailed CRS purpose codes in the sector field
---------------------------------------------------------
**(a) Don’t use very broad codes**

Broad "multisector aid" or "sector not specified" purpose codes are not mappable to budgets and are too aggregate to tell you much that is useful about the activity. Publishers should not use these purpose codes if they want activities to be mappable to budgets.

List of multisector codes that should not be used (source `IATI 2012 Study on Better Reflecting Aid Flows in Country Budgets <http://www.aidtransparency.net/wp-content/uploads/2013/05/Study-on-better-reflecting-aid-flows-in-country-budgets.doc>`_, `Annex 4 <http://www.aidtransparency.net/wp-content/uploads/2013/05/Annex-4-Common-Code-and-CRS-Spreadsheet.xls>`_ - codes that are "not classifiable - multisector"):

* 43010 - Multisector aid
* 43050 - Non-agricultural alternative development
* 43081 - Multisector education / training
* 43082 - Research / scientific institutions
* 52010 - Food aid/food security programmes
* 99810 - Sectors not specified

**(b) Use the more detailed "voluntary" CRS purpose codes, not “parent” codes**

In a fairly broad sample of 35-40 countries, various studies found that more disaggregated ("voluntary") codes under 15 existing CRS purpose codes were needed to map to budgets. Publishers should use the voluntary codes instead of the "parent" codes if they want their activities to be mappable to budgets.

The CRS purpose codes, including the more detailed voluntary codes, are listed in the `DAC and CRS codelists Excel sheet <http://www.oecd.org/dac/financing-sustainable-development/development-finance-standards/DAC-CRS-CODES.xls>`_ .

The additional codes were `approved by WP-STAT under the written procedure <http://www.oecd.org/officialdocuments/publicdisplaydocumentpdf/?cote=DCD/DAC/STAT(2015)30/REV1&docLanguage=En>`_ in February 2016. The `IATI Steering Committee approved the use of the more detailed CRS purpose codes <http://www.aidtransparency.net/wp-content/uploads/2013/01/Paper-4c-from-TAG-Working-Group-on-Budget-Identifier.pdf>`_ (instead of using the “Common Code" codelist) in March 2014.

