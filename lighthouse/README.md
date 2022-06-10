zlobniyshurik.lighthouse
=========

Copy **[Lighthouse](https://github.com/VKCOM/lighthouse)** GUI for `Clickhouse` from GitHub to local catalog

Requirements
------------

Tested with `RHEL 8.x` clones.  

In theory can work with `Fedora` and `RHEL 9.x` (RPM-based OSes with **dnf** package manager)

Role Variables
--------------

***[defaults/main.yml](./defaults/main.yml)***
| Variables | Description | Default settings |
| :--------  | :----------   | :------------  |
| **`lighthouse_git_folder`** | Catalog for .git-part of `Lighthouse` | **/tmp/lighthouse.git** |
| **`lighthouse_url`** | URL for GitHub `Lighthouse` repo | **https://github.com/VKCOM/lighthouse.git** |
| **`lighthouse_version`** | git-branch in `Lighthouse` repo | **master** |
| **`lighthouse_web_folder`** | Catalog for web-part of `Lighthouse` | **/tmp/lighthouse.git** |

Dependencies
------------

No dependencies

Example Playbook
----------------

**playbook**

    - hosts: servers
      roles:
         - { role: zlobniyshurik.lighthouse }

License
-------

MIT

Author Information
------------------

Alexander Dyadyun  
zlobniyshurik@gmail.com
