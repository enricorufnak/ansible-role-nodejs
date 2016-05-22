[![Build Status](https://travis-ci.org/enricorufnak/ansible-role-nodejs.svg?branch=master)](https://travis-ci.org/enricorufnak/ansible-role-nodejs)

Ansible Role: Node.js
=====================

Install Node.js on Ubuntu.

Requirements
------------

None.

Role Variables
--------------

Available variables are listed below, along with default values:

    nodejs_version: "5.x"

Node.js version to install. Default is "5.x" and other possible versions are "0.10" and "4.x"

    nodejs_npm_global_packages: []

Add a list of npm packages with a name and version (optional) to be installed globally. Example see below:

    nodejs_npm_global_packages:
          # Install a specific version
          - name: gulp
            version: 3.9.1
          # Install the latest stable release
          - name: laravel-elixir


Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: enricorufnak.nodejs }

License
-------

MIT

Author Information
------------------

This role was created in 2016 by [Enrico Rufnak](http://www.rufnak.de)