# Self Ansible

Project for setting up my own hosts with Ansible. This will also serve as a replacement to my half finished [standalone puppet][standalone puppet]

## Goals

- [ ] Install common packages
 - [X] git
 - [X] lzma
 - [X] wireshark
 - [X] meld
 - [X] chromium-browser
 - [ ] curl
 - [ ] vim-full
- [ ] Setup i3
 - [ ] Install packages: i3, i3lock, xbacklight and conky
- [ ] Setup dotfiles using freshrc
- [ ] Install docker and configure where necessary
- [ ] Configure [locale][locale gist]

### Do these later

These would need some changing of my fresh rc configurations:

- [ ] Configure ruby development environment
- [ ] Configure node version managed environment

## Running this Ansible playbook

```sh
sudo apt-get install software-properties-common -y
sudo apt-add-repository -y ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible git -y
mkdir ~/Dev/ -p
git clone https://github.com/steakunderscore/self-ansible.git ~/Dev/self-ansible
cd ~/Dev/self-ansible
ansible-playbook localhost site.yml
```

[standalone puppet]: https://github.com/steakunderscore/standalone-puppet
[locale gist]: https://gist.github.com/steakunderscore/5bd9271b4866fe9467aeacaefa21b0cc
