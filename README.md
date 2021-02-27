Role Name
=========

Role for initial server setup: Install required packages, sshd and sudo configuration

Requirements
------------

None.

Role Variables
--------------

Available variables:
 - `create_user` - Create custom user or not (Default: `True`)
   **Note:** If this variable set to `False`, set `permit_root_login` to `yes`
 - `username` - Username of custom user (Default: `server`)
 - `ssh_key` - Path to ssh public key (Default: `$HOME/.ssh/id_ecdsa`)
 - `ssh_port` - Port in `sshd_config` (Default: `22`)
 - `permit_root_login` - PermitRootLogin in `sshd_config` (Default: `no`)
 - `max_auth_tries` - MaxAuthTries in `sshd_config` (Default: `5`)
 - `password_authentication`: PasswordAuthentication in `sshd_config` (Default: `no`)
 - `setup_firewall` Setup firewall or not (Default: `True`)

Dependencies
------------

None.

License
-------

GPLv3

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
