Role Name
=========

Setups up vnc

Requirements
------------

Currently, assumes vnc and x11 is installed

Role Variables
--------------

* VNC_PASSWORD_METHOD, the password method; Currently, the only supported method is 'vncpassword'
* VNC_USERS, array of username and display numbers to setup. E.g.

VNC_USERS:
  user1:
    display_number: 1
    password: xyz123
  user2:
    display_number: 2
    password: uvw456

Also, if /home/{{ VNC_USER.username}} does not exist, it will skip setting up vnc for a user

Dependencies
------------


License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
