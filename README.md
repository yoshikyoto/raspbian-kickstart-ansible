# Raspbian kickstart Ansible

Ansible after install raspbian (for Raspberry Pi).

## Execute

1. Change `roles/ssh-config/files/authorized_keys` into your publickey, correctly.
2. Change `inventory` and your raspbian's IP adress in it.
3. Execute `ansible-playbook playbooks/kickstart.yml`

## What's this?

Raspbian has `pi` user (password is `raspberry`) just after installed.

Using this Ansible playbook, You can ssh `pi` user from your PC by publikey authentication.
And disable password authentication (for Security. Everyone knows `pi` use has password `raspberry`).
