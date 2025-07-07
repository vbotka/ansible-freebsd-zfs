====================================
vbotka.freebsd_zfs 2.7 Release Notes
====================================

.. contents:: Topics


2.7.3
=====

Release Summary
---------------
Update README.


2.7.2
=====

Release Summary
---------------
Update README.


2.7.1
=====

Release Summary
---------------
Maintenance update.

Major Changes
-------------

Minor Changes
-------------
* Remove unused variable fzfs_backup_conf
* Run tasks/debug.yml first.
* Update tasks/facts.yml. Always get zpool facts.


2.7.0
=====

Release Summary
---------------
Ansible 2.18 update

Major Changes
-------------
* Support FreeBSD 13.4, 13.5, 14.2, 14.3
* Add tasks/pools.yml Add dictionary fzfs_pools
* Use module community.general.sysrc
* Use module vbotka.freebsd.service instead of ansible.builtin.service
* Update handlers to use the module vbotka.freebsd.service
* Collection vbotka.freebsd is required.

Minor Changes
-------------
* .gitignore added to version control.
* Improved tasks formatting.
* Added var fzfs_assert_quiet (default=true).
* Added vars to debug in tasks/facts.yml
* Added var fzfs_facts_ds (default=false). Getting datasets is optional.
* Added pools sanity.

Bugfixes
--------

Breaking Changes / Porting Guide
--------------------------------
* The role vbotka.freebsd.postinstall from the collection vbotka.freebsd is required instead of the
  standalone role vbotka.freebsd_postinstall (note the dot '.' instead of the underscore '_' in the
  role's name.
* The variable fzfs_assert_enable (default=true) was removed. The sanity tasks are enabled
  by default.
