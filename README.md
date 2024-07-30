# [molecule_test](#molecule_test)

Example Ansible role for testing with molecule.

| GitHub                               | Version                                 | License                                 | Ansible Galaxy                   | Downloads                               |
|--------------------------------------|-----------------------------------------|-----------------------------------------|----------------------------------|-----------------------------------------|
|[![github][github-badge]][github-link]|[![version][version-badge]][version-link]|[![license][license-badge]][license-link]|[![role][galaxy-badge]][galaxy-link]|[![downloads][download-badge]][download-link]|

[github-link]: https://github.com/ucomesdag/ansible-role-molecule_test/actions
[version-link]: https://github.com/ucomesdag/ansible-role-molecule_test/releases
[license-link]: https://github.com/ucomesdag/ansible-role-molecule_test/LICENSE
[galaxy-link]: https://galaxy.ansible.com/ui/standalone/roles/ucomesdag/molecule_test/
[download-link]: https://galaxy.ansible.com/ui/standalone/roles/ucomesdag/molecule_test/versions/


[github-badge]: https://github.com/ucomesdag/ansible-role-molecule_test/workflows/Ansible%20Molecule/badge.svg
[version-badge]: https://img.shields.io/github/v/release/ucomesdag/ansible-role-molecule_test?include_prereleases&label=Release
[license-badge]: https://img.shields.io/github/license/ucomesdag/ansible-role-molecule_test?label=License
[galaxy-badge]: https://img.shields.io/badge/Ansible-Galaxy-blue?style=flat&logo=ansible&logoColor=white&color=5bbcbf
[download-badge]: https://img.shields.io/ansible/role/d/ucomesdag/molecule_test?label=Role%20Downloads

## [Example Playbook](#example-playbook)

This example is taken from `molecule/resources/converge.yml` and is tested on each push, pull request and release.

```yaml
---
- name: Converge
  hosts: all
  become: yes
  gather_facts: no

  roles:
    - role: ucomesdag.molecule_test
```

## [Role Variables](#role-variables)

These variables are set in `defaults/main.yml`:

```yaml
---
# defaults file for molecule_test

# The webpage content
molecule_test_webpage_content: Hello world!
```

## [Dependencies](#dependencies)

Overview of role dependencies:

![dependencies](https://raw.githubusercontent.com/ucomesdag/ansible-role-molecule_test/png/requirements.png "Dependencies")

## [Requirements](#role-requirements)

- pip packages listed in [requirements.txt](https://github.com/ucomesdag/ansible-role-molecule_test/blob/master/requirements.txt).

## [Compatibility](#compatibility)

This role has been tested on these [container images](https://quay.io/user/ucomesdag):

|container      |tags                            |
|---------------|--------------------------------|
|almalinux      |latest, 8                       |
|alpine         |latest, edge                    |
|amazonlinux    |latest, 2                       |
|archlinux      |latest                          |
|centos         |latest                          |
|debian         |latest, trixie, bullseye,buster |
|fedora         |latest, rawhide, 40, 39         |
|opensuse       |latest, tumbleweed              |
|rhel           |latest, ubi8                    |
|rocky          |latest, 8                       |
|rpi-os         |latest                          |
|ubuntu         |latest, jammy, focal, bionic    |

The minimum version of Ansible required is 2.16, tests have been done to:

- The previous version (2.16).
- The current version (2.17).
- ~~The development version (2.18 is unreleased).~~

See the [Ansible community changelogs](https://docs.ansible.com/ansible/devel/reference_appendices/release_and_maintenance.html#ansible-community-changelogs) for details.

## [Exceptions](#exceptions)

Some variations of the build matrix do not work. These are the variations and reasons why the build won't work:

| variation | reason                                                                                      |
|-----------|---------------------------------------------------------------------------------------------|
| py.*-2.17 | Ansible 2.17 requires python 3.8 or newer and will fail run on systems with older versions. |


If you find issues, please register them in [GitHub](https://github.com/ucomesdag/ansible-role-molecule_test/issues)

## [License](#license)

Apache-2.0
