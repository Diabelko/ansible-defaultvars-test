This repo is just a simple testcase of Ansible default variable value handling.

According to the [documentation](https://docs.ansible.com/ansible/latest/user_guide/playbooks_reuse_roles.html#using-roles), Ansible will include all defaults/main.yaml contents in the play.

A role named test-B doesn't have a default value defined for `testvar` and yet it is accessible and its value is equal to value from test-C role.

To run it, type: `ansible-playbook test.yaml -i localhost, -c local`
