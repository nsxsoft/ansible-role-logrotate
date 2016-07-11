# ansible-role-logrotate

[![Build Status](https://travis-ci.org/linuxhq/ansible-role-logrotate.svg?branch=master)](https://travis-ci.org/linuxhq/ansible-role-logrotate)

RHEL/CentOS - Rotates, compresses, and mails system logs

## Requirements

None

## Role Variables

Available variables are listed below, along with default values:

    logrotate_compress: False
    logrotate_create: True
    logrotate_dateext: True
    logrotate_include: /etc/logrotate.d
    logrotate_interval: weekly
    logrotate_weeks: 4

## Dependencies

None

## Example Playbook

    - hosts: servers
      roles:
        - role: linuxhq.logrotate
          logrotate_compress: True
          logrotate_interval: daily
          logrotate_weeks: 1

## License

BSD

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
