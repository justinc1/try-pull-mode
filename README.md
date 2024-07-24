# try-pull-mode

Demo for Ansible pull-mode.
See https://docs.ansible.com/ansible/latest/cli/ansible-pull.html.

We need
- playbook to create demo VM
- playbook to setup and maintain demo VM

Usage:

One time setup:

```bash
python3 -m venv .venv
source .venv/bin/activate

cat >>env.sh <<EOF
export SC_HOST=https://1.2.3.4
export SC_USERNAME=admin
export SC_PASSWORD=admin
EOF
source env.sh

pip install -r requirements.txt
ansible-galaxy install -r requirements.yml
```
