====================================
vbotka.freebsd_zfs 2.6 Release Notes
====================================

.. contents:: Topics
# BEGIN Commits 2.6.3
- ''
# END Commits 2.6.3
# BEGIN Release notes 2.6.3
2.6.3
=====
Release Summary
---------------
Major Changes
-------------
Minor Changes
-------------
Bugfixes
--------
Breaking Changes / Porting Guide
--------------------------------
# END Release notes 2.6.3


2.6.2
=====

Release Summary
---------------
Maintenance update.

Major Changes
-------------
* Add tasks sysctl.yml

Minor Changes
-------------
* Update README
* Update vars/main.yml.sample


2.6.1
=====

Release Summary
---------------
Ansible 2.17 update

Major Changes
-------------
* Add supported 14.1

Minor Changes
-------------
* Update README
* Update debug.yml
* Add var fzfs_role_version
* Add var fzfs_debug2 default=false
* Update facts.yml. Remove facts_include_1.yml

Bugfixes
--------

Breaking Changes / Porting Guide
--------------------------------
* Structure of fzfs_datasets changed. See facts.yml


2.6.0
=====

Release Summary
---------------
Ansible 2.16 update

Major Changes
-------------
* Supported FreeBSD: 13.3, 14.0

Minor Changes
-------------
* Update README
* Update Ansible lint config.
* Fix Ansible lint.

Bugfixes
--------

Breaking Changes / Porting Guide
--------------------------------
