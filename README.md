<a href="https://www.bitbull.ch"><img src="https://www.bitbull.ch/wiki/images/teamwork-trans.png" alt="Bitbull" width="250px"/></a>

# joe-speedboat.guacamole
This Ansible Role is installing and configuring Guacamole HTML5 Gateway
* `Mariadb`
* `Tomcat`
* `Guacamole via RPM`
* `Guacamole extensions: default/main.yml`
* `Nginx reverse proxy`

## Ansible Setup/Deps
```bash
curl -L ansible.bitbull.ch | bash
```

## Install role and deps with ansible-galaxy:
```bash
ansible-galaxy install joe-speedboat.guacamole
```

## Install role with git:
```bash
git clone https://github.com/joe-speedboat/ansible.guacamole.git /etc/ansible/roles/joe-speedboat.guacamole
```

## Requirements
* Ansible 3.11 or higher is required for this Ansible Role
* OS Releases:
  * Rocky Linux 8
  * Rocky Linux 9
  * other RHELish OS may work, but are not tested

## Role dependencies
* mariadb role
```bash
ansible-galaxy role install -r roles/requirements.yml
```

## Collection depencies
* community.mysql from mariadb role
```bash
ansible-galaxy collection install -r collections/requirements.yml
```

## Role Variables
Variables are self speaking or documented in:   
* `defaults/main.yml`
* `vars/main.yml`

## Example Playbook
Example playbooks for this role are located in ´test´ folder:
* `tests/install_guacamole.yml`

## License
https://opensource.org/licenses/LGPL-3.0    
Copyright (c) Chris Ruettimann <chris@bitbull.ch>

