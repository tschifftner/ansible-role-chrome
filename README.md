## This role is DEPRECATED!

# Ansible Role: Install chrome

[![Build Status](https://travis-ci.org/tschifftner/ansible-role-chrome.svg?branch=master)](https://travis-ci.org/tschifftner/ansible-role-chrome)

Installs [chrome](https://www.google.com/chrome) browser on Debian/Ubuntu linux servers.

## Requirements

none

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
chrome_apt_keyurl: 'https://dl-ssl.google.com/linux/linux_signing_key.pub'

chrome_apt_repositories:
  - 'deb http://dl.google.com/linux/chrome/deb/ stable main'

chrome_apt_packages:
  - 'google-chrome-stable'
```

## Dependencies

None.

## Installation

```
$ ansible-galaxy install tschifftner.chrome
```

## Example Playbook

    - hosts: server
      roles:
        - { role: tschifftner.chrome }

## Supported OS
## Supported OS
Ansible          | Debian Jessie    | Ubuntu 14.04    | Ubuntu 12.04
:--------------: | :--------------: | :-------------: | :-------------: 
2.1              | Yes              | Yes             | Yes


## License

[MIT License](http://choosealicense.com/licenses/mit/)

## Author Information

 - [Tobias Schifftner](https://twitter.com/tschifftner), [ambimax® GmbH](https://www.ambimax.de)
