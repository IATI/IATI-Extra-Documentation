
.. image:: https://github.com/IATI/IATI-Extra-Documentation/workflows/CI_version-2.03/badge.svg
    :target: https://github.com/IATI/IATI-Extra-Documentation/actions

This is the repsitory contains additional documentation about the IATI Standard, and is part of IATI Standard Single Source of Truth (SSOT). For more detailed information about the SSOT, please see https://github.com/IATI/IATI-Standard-SSOT/blob/master/meta-docs/index.rst 

Whilst this is the single source for the documentation, it is probably easier to read it integrated into the website, e.g. at http://iatistandard.org/activity-standard/

This repository is currently under development, and does not necessarily represent any current or future version of the IATI standard.

Markup
^^^^^^

The markup in this repository is restructured text, for more information see http://sphinx-doc.org/rest.html

If you are creating a new file, please use the ``.rst`` extension, to let GitHub know the file is restructured text. You may need to create the file (and commit it), and edit again before GitHub will offer you the preview button (at the top of the editor), so you can see what your formatting will look like as you edit a file.

Headings
========

Headings are created by 'underlining' with one of the special characters e.g. ``^`` ``=`` and ``-``, e.g.::

    Headings
    ========

The same character should be used for all headings of a given level. The level of a heading will be inferred automatically from the ordering in the document (ie. the first heading type found is level 1 etc.)

Internal links
==============

Internal links can be created using the ``:doc:`` directive. e.g.::

    Additionally, a :doc:`region vocabulary </codelists/RegionVocabulary>` can also be declared in this element

Note that the file extension is absent.

Spell Checking
^^^^^^^^^^^^^^

The default github editor does not have spell checking, as its syntax highlighting interferes. However, if you turn on Zen mode (full screen), you will get your browser's spell checking.

.. image:: https://f.cloud.github.com/assets/296432/93884/91f64d16-6638-11e2-97d2-4c8f4cdbe4d2.png

