# Ansible Role - SonarQube

[![MIT licensed](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![GitHub last commit (branch)](https://img.shields.io/github/last-commit/wolffaxn/ansible-role-sonarqube/master.svg)](https://github.com/wolffaxn/ansible-role-sonarqube)

## About

Installs SonarQube for RedHat/CentOS linux servers.

## Requirements

None.

## Role Variables

Available variables are listed below, along with default values:

    sonar_version: 6.0

    sonar_download_dir: /tmp
    sonar_download_cleanup: true
    sonar_install_dir: /opt

    sonar_database: postgresql

    sonar_database_name: sonar
    sonar_database_host: localhost
    sonar_database_port: "5432"

    sonar_database_username: sonar
    sonar_database_password: sonar

## Dependencies

None.

## Example Playbook

For RHEL / CentOS

```yaml
---
- hosts: localhost
  become: true
  become_method: sudo
  remote_user: root
  roles:
    - ansible-role-sonarqube
```
## License

This project is licensed under the terms of the [MIT license](LICENSE).
