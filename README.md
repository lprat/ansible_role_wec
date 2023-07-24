Role Name
=========

Ansible role to install server wec according by palantir method (https://github.com/palantir/windows-event-forwarding)

Role Variables
--------------

 - sha1_dll: hash of local file (in files dir)  CustomEventChannels.dll (source: https://github.com/palantir/windows-event-forwarding/tree/master/windows-event-channels)
 - sha1_man: hash of local file (in files dir)  CustomEventChannels.man (source: https://github.com/palantir/windows-event-forwarding/tree/master/windows-event-channels)
 - path_temp: path remote to upload files dll/man/xml (default: c:\Temp)
 - wecsvc_events_maxsize: size of logs (default: 4GB - in bytes)
 - wef_palantir_subscriptions: palantir subscription list (name is same of filename xml - https://github.com/palantir/windows-event-forwarding/tree/master/windows-event-channels)

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: wef

License
-------

Apache 2.0

Author Information
------------------

Contact: lionel.prat9@gmail
