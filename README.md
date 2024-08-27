# laptop-provision
An initial attempt at automating laptop provisioning with Ansible. Especially
useful after getting a new laptop or installing the OS from scratch.

I'm assuming that I'll stick with Ubuntu. If this changes in the future, I may
need to change a few things.

To start provisioning a brand new laptop:
```bash
sudo apt-add-repository --yes --update ppa:ansible/ansible
sudo apt install ansible
wget https://github.com/tayken/laptop-provision/archive/refs/heads/main.zip
unzip main.zip
cd laptop-provision-main
ansible-playbook main.yml --ask-become-pass
```
