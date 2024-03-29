# freebsd_zfs

[![quality](https://img.shields.io/ansible/quality/27910)](https://galaxy.ansible.com/vbotka/freebsd_zfs)[![Build Status](https://travis-ci.org/vbotka/ansible-freebsd-zfs.svg?branch=master)](https://travis-ci.org/vbotka/ansible-freebsd-zfs)

[Ansible role.](https://galaxy.ansible.com/vbotka/freebsd_zfs/) FreeBSD. Configure ZFS.

Feel free to [share your feedback and report issues](https://github.com/vbotka/ansible-freebsd-zfs/issues).

[Contributions are welcome](https://github.com/firstcontributions/first-contributions).


## Requirements

### Roles

* [vbotka.freebsd_postinstall](https://galaxy.ansible.com/vbotka/freebsd_postinstall)

This role is needed to run tasks from *sysctl.yml* and *loader.yml*

### Collections

* community.general


## Variables

Review defaults and examples in vars.


## Workflow

1) Change shell to /bin/sh

```
shell> ansible host -e 'ansible_shell_type=csh ansible_shell_executable=/bin/csh' -a 'sudo pw usermod user -s /bin/sh'
```

2) Install the role and dependencies

```
shell> ansible-galaxy role install vbotka.freebsd_zfs
shell> ansible-galaxy role install vbotka.freebsd_postinstall
shell> ansible-galaxy collection install community.general
```

3) Fit variables, e.g. in vars/main.yml

```
shell> editor vbotka.freebsd_zfs/vars/main.yml
```

4) Create playbook

```
shell> cat freebsd-zfs.yml
- hosts: host
  roles:
    - vbotka.freebsd_zfs
```

5) Configure the system

```
shell> ansible-playbook freebsd-zfs.yml
```


## References

- [FreeBSD handbook: Chapter 19. ZFS](http://www.freebsd.org/doc/handbook/zfs.html)
- [FreeBSD wiki: ZFS](https://wiki.freebsd.org/ZFS)
- [FreeBSD wiki: ZFS Quick Start Guide](https://wiki.freebsd.org/ZFSQuickStartGuide)
- [FreeBSD wiki: ZFS Tuning Guide](https://wiki.freebsd.org/ZFSTuningGuide)
- [FreeBSD wiki: Category ZFS](https://wiki.freebsd.org/CategoryZfs)


## License

[![license](https://img.shields.io/badge/license-BSD-red.svg)](https://www.freebsd.org/doc/en/articles/bsdl-gpl/article.html)


## Author Information

[Vladimir Botka](https://botka.info)
