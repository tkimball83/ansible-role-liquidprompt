# ansible-role-liquidprompt

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-liquidprompt.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-liquidprompt)

macOS - A useful adaptive prompt for bash & zsh

## Requirements

This role requires Homebrew to be installed

## Role Variables

Available variables are listed below, along with default values:

    liquidprompt_battery_threshold: 75
    liquidprompt_enable_batt: True
    liquidprompt_enable_bzr: True
    liquidprompt_enable_fossil: True
    liquidprompt_enable_fqdn: False
    liquidprompt_enable_git: True
    liquidprompt_enable_hg: True
    liquidprompt_enable_jobs: True
    liquidprompt_enable_load: True
    liquidprompt_enable_perm: True
    liquidprompt_enable_proxy: True
    liquidprompt_enable_runtime: False
    liquidprompt_enable_scls: True
    liquidprompt_enable_screen_title: False
    liquidprompt_enable_shorten_path: True
    liquidprompt_enable_ssh_colors: False
    liquidprompt_enable_sudo: False
    liquidprompt_enable_svn: True
    liquidprompt_enable_temp: True
    liquidprompt_enable_time: False
    liquidprompt_enable_title: True
    liquidprompt_enable_vcs_root: False
    liquidprompt_enable_virtualenv: True
    liquidprompt_hostname_always: '0'
    liquidprompt_load_threshold: 60
    liquidprompt_path: /usr/local/share/liquidprompt
    liquidprompt_path_keep: 2
    liquidprompt_path_length: 35
    liquidprompt_percents_always: True
    liquidprompt_runtime_threshold: 2
    liquidprompt_temp_threshold: 60
    liquidprompt_time_analog: False
    liquidprompt_user_always: True

The following are additional variables, not defined by default:

    liquidprompt_dest: /Users/tkimball
    liquidprompt_disabled_vcs_path: []
    liquidprompt_group: staff
    liquidprompt_owner: tkimball
    liquidprompt_ps1_file: /path/to/file.ps1
    liquidprompt_source: /path/to/file.theme

## Dependencies

None

## Example Playbook

    - hosts: localhost
      connection: local
      roles:
        - role: tkimball83.liquidprompt
          liquidprompt_battery_threshold: 50
          liquidprompt_enable_time: True

## License

BSD

## Author Information

This role was created by [Taylor Kimball](http://www.linuxhq.org).
