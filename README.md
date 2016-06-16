# Self Ansible

Project for setting up my own hosts with Ansible. This will also serve as a replacement to my half finished [standalone puppet][standalone puppet]

## Goals

- [ ] Install common packages
 - [X] Git
 - [X] lzma
 - [X] wireshark
 - [X] meld
 - [X] chromium-browser
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
sudo apt-get install software-properties-common
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
mkdir ~/Dev/
git clone https://github.com/steakunderscore/self-ansible.git ~/Dev/self-ansible
ansible-playbook localhost site.yml
```

[standalone puppet]: https://github.com/steakunderscore/standalone-puppet
