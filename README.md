Role Name
=========

Triggers a Jenkins build job

Requirements
------------

None.

Role Variables
--------------

Variables that need to be set:
```yaml
jenkins:
  host: 
  user: 
  passwd: 
  token: 
  job: 
```

Where: 
`host` is the url at which the jenkins server can be reached.

`user` is the jenkins server user allowed to trigger the build. 

`passwd` is the password associated to `user`.

`token` is the api token given to `user`.

`job` is the name of the job to trigger.


Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
- hosts: servers
  vars:
    jenkins:
      host: www.example.com 
      user: myUser 
      passwd: myPasswd 
      token: token 
      job: MyJob 
  roles:
     - ansible_role_jenkins_build_trigger
```
License
-------

BSD

Author Information
------------------

Created by Vincent D-Gauthier
