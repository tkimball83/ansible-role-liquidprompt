# ansible-role-liquidprompt

[![Build Status](https://travis-ci.org/tkimball83/ansible-role-liquidprompt.svg?branch=master)](https://travis-ci.org/tkimball83/ansible-role-liquidprompt)
[![Ansible Galaxy](https://img.shields.io/badge/ansible--galaxy-liquidprompt-blue.svg?style=flat)](https://galaxy.ansible.com/tkimball83/liquidprompt)
[![License](https://img.shields.io/badge/license-GPLv3-brightgreen.svg?style=flat)](COPYING)

macOS - A useful adaptive prompt for bash & zsh

## Requirements

This role requires homebrew to be installed

## Role Variables

Available variables are listed below, along with default values:

    liquidprompt_battery_threshold: 75
    liquidprompt_dest: "{{ ansible_env.HOME }}"
    liquidprompt_disabled_vcs_path: []
    liquidprompt_enable_batt: true
    liquidprompt_enable_bzr: true
    liquidprompt_enable_fossil: true
    liquidprompt_enable_fqdn: false
    liquidprompt_enable_git: true
    liquidprompt_enable_hg: true
    liquidprompt_enable_jobs: true
    liquidprompt_enable_load: true
    liquidprompt_enable_perm: true
    liquidprompt_enable_proxy: true
    liquidprompt_enable_runtime: false
    liquidprompt_enable_scls: true
    liquidprompt_enable_screen_title: false
    liquidprompt_enable_shorten_path: true
    liquidprompt_enable_ssh_colors: false
    liquidprompt_enable_sudo: false
    liquidprompt_enable_svn: true
    liquidprompt_enable_temp: true
    liquidprompt_enable_time: false
    liquidprompt_enable_title: true
    liquidprompt_enable_vcs_root: false
    liquidprompt_enable_virtualenv: true
    liquidprompt_group: "{{ ansible_effective_group_id }}"
    liquidprompt_hostname_always: '0'
    liquidprompt_load_threshold: 60
    liquidprompt_owner: "{{ ansible_effective_user_id }}"
    liquidprompt_path: /usr/local/share/liquidprompt
    liquidprompt_path_keep: 2
    liquidprompt_path_length: 35
    liquidprompt_percents_always: true
    liquidprompt_ps1_file: ''
    liquidprompt_runtime_threshold: 2
    liquidprompt_source: []
    liquidprompt_temp_threshold: 60
    liquidprompt_time_analog: false
    liquidprompt_user_always: true

## Dependencies

None

## Example Playbook

    - hosts: localhost
      connection: local
      roles:
        - role: tkimball83.liquidprompt
          liquidprompt_battery_threshold: 50
          liquidprompt_enable_time: true

## License

Copyright (C) 2018 Taylor Kimball <tkimball@linuxhq.org>

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
along with this program. If not, see <http://www.gnu.org/licenses/>.
