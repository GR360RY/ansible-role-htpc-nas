htpc-nas
===========
<!-- [![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--nas-green.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/) -->

An Ansible role to setup and configure NAS functionality ( NFS, CIFS and AFP ) for HTPC Server under Debian based distro's.

Role Variables
--------------

Dependencies
------------

 Role Name| Description
----------|-----------
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--user-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4645) | Create htpc user on Linux.
[![Galaxy](http://img.shields.io/badge/galaxy-GR360RY.htpc--media-blue.svg?style=flat-square)](https://galaxy.ansible.com/list#/roles/4926)| Create HTPC Media Folders.

Variables defined in `GR360RY.htpc-user` role:

 GR360RY.htpc-user        | Required   | Default       | Comment          
--------------------------|:----------:|---------------|---------
 htpc_user_username       | no         | htpc          |
 htpc_user_password       | no         | htpc          |
 htpc_user_shell          | no         | /bin/bash     |
 htpc_user_sudo_access    | no         | yes           |

Variables defined in `GR360RY.htpc-media` role:

 GR360RY.htpc-media       | Required   | Default       | Comment          
--------------------------|:----------:|---------------|---------
 htpc_media_path          | no         | /mnt/media    |
 htpc_media_movies        | no         | movies        |
 htpc_media_tv            | no         | tv            |
 htpc_media_music         | no         | music         |
 htpc_media_pictures      | no         | pictures      |

License
-------

BSD

Author Information
------------------

Gregory Shulov
