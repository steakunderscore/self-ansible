# Self Ansible

Project for setting up my own hosts with Ansible. This will also serve as a replacement to my half finished [standalone puppet][standalone puppet]

## Goals

- [ ] Install common packages
 - [ ] Git
- [ ] Set i3
 - [ ] Install packages: i3, i3lock, xbacklight and conky
- [ ] Setup dotfiles using freshrc
- [ ] Install docker and configure where necessary

### Do these later

These would need some changing of my fresh rc configurations:

- [ ] Configure ruby development environment
- [ ] Configure node version managed environment

## Running this Ansible playbook

```sh
ansible-playbook localhost site.yml
```

[standalone puppet]: https://github.com/steakunderscore/standalone-puppet
