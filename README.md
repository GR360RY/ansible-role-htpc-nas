htpc-nas
===========
<!-- [![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--nas-green.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/) -->

An Ansible role to setup and configure NAS functionality ( NFS, CIFS and AFP ) for HTPC Server under Ubuntu.

Requirements
------------

This role requires Ansible 1.6 or higher. Platform requirements are listed in the metadata file.


Overview
--------


Role Variables
--------------


Dependencies
------------

 Role Name| Description
----------|-----------
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--user-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645) | Create htpc user on Linux.

Variables defined in `GR360RY.htpc-user` role:

 GR360RY.htpc-user        | Required   | Default       | Comment          
--------------------------|:----------:|---------------|---------
 htpc_user_username       | no         | htpc          |
 htpc_user_password       | no         | htpc          |
 htpc_user_shell          | no         | /bin/bash     |
 htpc_user_sudo_access    | no         | yes           |

HTPC-Ansible Project
--------------------

This role is part of HTPC-Ansible project that includes additional roles for building Ubuntu Based HTPC Server.

 Role name               | Comment
-------------------------|-----------------------------
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--user-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645) |  Create htpc user on Linux
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--media-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)      | Create htpc media folders
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--nas-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Configure NAS ( NFS, CIFS and AFP )
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.kodi--client-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/3098)    | Install Kodi Media Player
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.kodi--mysql-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Install MySQL Backend for Kodi
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.deluge-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Install Deluged Bittornet Client
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.sabnzbd-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Install Sabnzbd
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.nzbtomedia-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Install NZBtoMedia Postprocessing
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.sickbeard-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Install SickRage
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.couchpotato-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Install CouchPotato
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--manager-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Install htpc-manager
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.tvheadend-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645)    | Install Tvheadend


Additional Info is available at [www.htpc-ansible.org](http://www.htpc-ansible.org)

License
-------

BSD

Author Information
------------------

Gregory Shulov