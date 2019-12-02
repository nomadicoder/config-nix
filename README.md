# config-nix
Configure personal machines

```
sudo apt-get install software-properties-common git
sudo apt-add-repository ppa:ansible/ansible
sudo apt-get update
sudo apt-get install ansible
```

Provision the machine

```bash
sudo ansible-pull -U https://github.com/nomadicoder/config-nix.git
```

While in development, clone the config-nix repository

```bash
git clone https://github.com/nomadicoder/config-nix.git
cd config-nix
```

And provision the system. Edit config-nix/local.yml

```bash
ansible-playbook local.yml
```
