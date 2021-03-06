Things left to do for Ansible Commander 
========================================

STAGE1 REMAINING:

- comment uncommented functions
- expose groups over REST
- expose hosts over REST
- expose users over REST
- test for methods at REST layer
- write an ansible inventory (python) script that accesses the database
- make sure user can only edit their own password unless named admin
- only user named 'admin' can add, rename other users, or delete users
- 'admin' account is not deleteable
- when adding a host and the host is not in any groups, create 'ungrouped' as a group if it does not exist
  and it there.  Similarly, when clearing host groups to zero, add to 'ungrouped'.  Requirement of inventory
  script.  When ungrouped groups to 0 hosts, delete 'ungrouped'

STAGE2:
- Foundation or Bootstrap skeleton of GUI app
- Login dialog to get username/password
- Javascript MVC widgets list users and groups
- JS to add hosts
- JS to add hosts to groups
- JS to edit host variables
- JS to add groups
- JS to add groups to groups
- JS to edit group variables
- JS to view all variables set on a host
- JS to view/browse inventory
- Logout button

Bonus
=====

- ansible callback plugin to save latest facts for each system
- modify setup playbook to install plugins
- migration script to convert inventory of YAML users (who want to) to database
- documentation page for ansible.github.com (ideally with 1 or 2 screenshots)

Completed Thus Far
==================

- README/LICENSE
- flask hello world
- initial setup playbook (mostly)
- python code to access datalayer
- basic user class
- basic auth layer wired in to user class
- full group/host data modelling
- encrypt passwords
- verify behavior when deleting groups in a chain, for hosts and groups, do _groups get cleared on hosts, etc
- ability to edit parent and group variables directly and all the right things update
- hrefs in all the objects
- established basic routes
- expose users over rest

Future releases (possible)
==========================

- browse ansible playbook results
- dashboard of overall system happiness and so forth
- browse and edit playbook content (???)
- trigger ad-hoc execution (???)
- trigger playbook execution (???)
- activity log
- object history
- ...




