htpc-nas
===========
[![Build Status](https://travis-ci.org/GR360RY/ansible-role-htpc-nas.svg?branch=master)](https://travis-ci.org/GR360RY/ansible-role-htpc-nas) [![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--nas-green.svg)](https://galaxy.ansible.com/GR360RY/htpc-nas/)

An Ansible role to setup and configure NAS functionality ( NFS, CIFS and AFP ) for HTPC Server under Ubuntu.

Requirements
------------

This role requires Ansible 2.0 or higher. Platform requirements are listed in the metadata file.
Make sure to download roles specified in **Dependencies** section if role installed **not** with Ansible Galaxy.

Overview
--------

List of tasks that will be performed under `htpc-nas` role:

1. Configure NFS Server. Squash all users to `htpc_user_username` uid
2. Configure SAMBA Server. Create `htpc_user_username` samba identified by `htpc_user_password`
3. Configure AFP ( Netatalk ) server for sharing data with Macs.

Folders layout if used with default variable values:

```
/mnt/media/            # Path to share over NFS,CIFS and AFP
├── downloads               
│   ├── complete
│   └── incomplete
├── movies
├── music
├── pictures
└── tv
```

Role Variables
--------------

```
---
# defaults file for htpc-nas

htpc_nas_enabled: yes

htpc_nas_nfs: yes
htpc_nas_cifs: yes
htpc_nas_afp: yes
```

Dependencies
------------

* `GR360RY.htpc-common` role. Creates htpc user and media folders

```
# defaults file for htpc-common

htpc_user_username: htpc
htpc_user_password: htpc
htpc_user_group: htpc
htpc_user_shell: /bin/bash
htpc_user_sudo_access: yes
htpc_ssh_service: yes
htpc_create_media_folders: yes
htpc_zeroconf: yes
htpc_media_path: /mnt/media
htpc_media_movies: movies
htpc_media_tv: tv
htpc_media_music: music
htpc_media_pictures: pictures
htpc_downloads_complete: "{{ htpc_media_path }}/downloads/complete"
htpc_downloads_incomplete: "{{ htpc_media_path }}/downloads/incomplete"
```

HTPC-Ansible Project
--------------------

This role is part of HTPC-Ansible project that includes additional roles for building Ubuntu Based HTPC Server.

Complete list of Ansible Galaxy roles is below:

- [`GR360RY.htpc-common`](https://galaxy.ansible.com/GR360RY/htpc-common) - Create htpc user and media folders
- [`GR360RY.htpc-nas`](https://galaxy.ansible.com/GR360RY/htpc-nas) - Configure NAS ( NFS, CIFS and AFP )
- [`GR360RY.kodi-client`](https://galaxy.ansible.com/GR360RY/kodi-client) - Install Kodi Media Player
- [`GR360RY.kodi-mysql`](https://galaxy.ansible.com/GR360RY/kodi-mysql) - Install MySQL Backend for Kodi
- [`GR360RY.deluge`](https://galaxy.ansible.com/GR360RY/deluge) - Install Deluge Bittornet Client
- [`GR360RY.sabnzbd`](https://galaxy.ansible.com/GR360RY/sabnzbd) - Install Sabnzbd Usenet Client
- [`GR360RY.nzbtomedia`](https://galaxy.ansible.com/GR360RY/nzbtomedia) - Install NZBtoMedia Postprocessing
- [`GR360RY.sickrage`](https://galaxy.ansible.com/GR360RY/sickrage) - Install SickRage
- [`GR360RY.couchpotato`](https://galaxy.ansible.com/GR360RY/couchpotato) - Install CouchPotato
- [`GR360RY.htpc-manager`](https://galaxy.ansible.com/GR360RY/htpc-manager) - Install HTPCManager

Additional Info is available at [www.htpc-ansible.org](http://www.htpc-ansible.org)

License
-------

BSD

Author Information
------------------

Gregory Shulov