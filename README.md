# Install all requirements to use docker on server

### Quick Start
 - `pip install -r requirements.txt`
 - `cp .inv.yml inv.yml`
 - add your hosts in inv.yml
 - `ansible-playbook -i inv.yml main.yml`

If ansible user needs password add flags:
 - -k asks password for ssh-connection (need to install `sshpass program`)
 - -b becomes sudo
 - -K asks password to become sudo

In addition, it will create user "user" on server and do `ssh-copy-id` from current user on your computer
