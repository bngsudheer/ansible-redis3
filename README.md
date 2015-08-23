Role Name
=========

Installs Redis 3 on EL 7(Read CentOS 7). If you want more platforms to be
supported, send a pull request and create an issue in the tracker.

Requirements
------------

* No other requirements


Role Variables
--------------

* increase_limits : yes | no. If this variable is set to 'yes', the hard and soft limits for the user redis will be set to 20480 in /etc/security/limits.conf. Restart the system for this setting to take effect.


Dependencies
------------

* No dependencies


Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: bngsudheer.ansible-redis3, increase_limits: yes}

License
-------

BSD

Author Information
------------------
Sudheer Satyanarayana: sudheer.zzz@sudheer.net
Twitter: http://www.twitter.com/bngsudheer
