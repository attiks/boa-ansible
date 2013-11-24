# BOA ansible playbook

BOA is part of the [Drupal barracuda module](https://drupal.org/project/barracuda) and is used to set up a full hosting environment for Drupal 6 and 7 sites.

## How to test

cp hosts.example hosts
cp settings.yml.example settings.yml
cp site.yml.example site.yml

cd vagrant
vagrant up
ssh-copy-id vagrant@192.168.50.4
ansible vagrant1 -m ping -i hosts

ansible-playbook -i hosts site.yml

## Status

This is a work in progress and only some roles are implemented.
