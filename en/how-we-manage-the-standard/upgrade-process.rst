Upgrades
========

.. toctree::
	 :hidden:

	 how-we-manage-the-standard/versions
	 upgrade-changelogs/noncore-codelist-changelog
	 upgrade-changelogs/decimal-upgrade-to-2-03
	 upgrade-changelogs/decimal-upgrade-to-2-02
	 upgrade-changelogs/integer-upgrade-to-2-01
	 upgrade-changelogs/v1-upgrades/decimal-upgrade-to-1-05
	 upgrade-changelogs/v1-upgrades/decimal-upgrade-to-1-04
	 upgrade-changelogs/v1-upgrades/decimal-upgrade-to-1-03
	 upgrade-changelogs/v1-upgrades/decimal-upgrade-to-1-02

The IATI standard is a living entity that will require improvement over time.

The standard is a collection of XML schema, core codelists, non-core codelists, documentation and rules.

Changes to some or all of those parts of the standard will be driven by the suggestions and experiences of the publishers and users of IATI data. Minor (previously decimal) upgrades can be initiated by the `Governing Board <https://iatistandard.org/en/about/governance/who-runs-iati/>`__, following advice from the TAG Chair and the Technical Lead. Major upgrades can be initiated by the `Members’ Assembly <https://iatistandard.org/en/about/join-iati/members-assembly/>`__, following the advice from the Governing Board.

Any member of the IATI community can make a proposal (via `IATI Discuss <https://discuss.iatistandard.org/c/standard-management>`__), and each upgrade process will receive its own forum where proposals can be assigned. The forums allow for a public exchange on the merits of the proposals to take place.

The current process for upgrading the standard (details below) was agreed at the `2017 Members’ Assembly <https://iatistandard.org/documents/242/Paper-10-Proposed-revisions-to-the-IATI-Standard-upgrade-process.pdf>`__. For the previous upgrade process please see the `Previous Upgrade Process <http://iatistandard.org/upgrades/all-versions/previous-process>`__ page.

Note: The current standard upgrade process will follow the widely-adopted `Semantic Versioning specification <https://semver.org/>`__ at the next major upgrade.

Patches
~~~~~~~~~~~~~

Patches (previously minor changes) can cover backwardly-compatible bug fixes. Changes are carried out by the Technical Team under the approval of the Secretariat.

Following version 3.0.0, each patch will have a version number.

Patches can currently be tracked through the `IATI GitHub <https://github.com/IATI>`__ account.

More significant changes to the standard are handled via upgrades. There are two types of upgrades - minor upgrades and major upgrades.

Minor Upgrades
~~~~~~~~~~~~~~~~

Minor (previously decimal) upgrades can cover changes that are optional and backwardly compatible. The Governing Board is responsible for initiating, overseeing and approving the upgrade.

**Minor upgrades can include:** 

-  Bug-fixes, including resolution of spelling and grammar errors (where edits have implications for usage and/or meaning)

-  Modifications to core codelists

-  Minor additions to the standard which improve the functionality without introducing substantial new content

All changes will be optional and backwardly compatible.


Major Upgrades
~~~~~~~~~~~~~~~~

Major (previously integer) upgrades can cover non-backwardly compatible changes. The Members’ Assembly is responsible for initiating and approving the upgrade. The Governing Board is responsible for overseeing progress.

**Major upgrades can include:** 

-  Substantial additions to the Standard

-  New mandatory fields

-  Changes that are not backwardly compatible


Upgrade Procedure
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Major and minor upgrades will be conducted in two distinct phases:

1. **Content** (what).This refers to the real-world use case. What problem will the change solve.

2. **Technical implementation** (how). This refers refers to the translation of the content into the syntax required by schema/codelist/rule. How do we solve the problem?

Wherever possible, decisions on changes to the standard should be reached by consensus. This means an absence of active dissent amongst those involved in the consultation process. If consensus cannot be reached the matter will be referred to the Governing Board for its assistance in resolving the dispute. The Governing Board, taking note of advice from the TAG chair and the Technical Lead, may adjudicate on an unresolved dispute.

****Timeline****

The Governing Board will approve a timeline for each upgrade prepared by the technical team. The timeline will consist of the following phases:

1. **Content consultation**
	a. Proposals are submitted and discussed by the community on. (Consultations mentioned in all phases can be conducted on `IATI Discuss <https://discuss.iatistandard.org/c/standard-management>`__, conference calls and meetings of the TAG.)

2. **Content approval**
	a. The community attempts to reach consensus on the final content. Wherever possible this phase should take place at a full meeting of the TAG.
	b. The final content is submitted to the Governing Board (minor) or Members’ Assembly (major) for approval or resolution.

3. **Technical consultation**
	a. The technical team and community technical experts translate the agreed content into the syntax of the Standard.
	b. Consultations take place on the technical proposals.

4. **Technical approval**
	a. The community attempts to reach consensus on the final content.
	b. The final content is submitted to the Governing Board for approval or resolution.

5. **Technical Implementation**
	a. The technical team creates a new candidate version of the standard.
	b. The technical team updates all utilities and services maintained by IATI to be compatible with the new version.
	c. The candidate version is made available to the community for publisher and user testing.

6. **Final Approval**
	a. The Governing Board, following advice from the TAG Chair, approves the final version and announces a Go Live date.
	b. A changelog for each minor and major upgrade will be made available on the `Upgrades <http://iatistandard.org/upgrades>`__ section of the IATI Standard website.
