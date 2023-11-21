# Growthbook A/B testing

- [Ansible doc](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- [Growthbook doc](https://docs.growthbook.io)

## Roles
- [x] Essentials
- [x] Docker (latest)
- [x] Growthbook

## Setup
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run
- Add ssh config hostname to `hosts` .
- Add your server public ip to `APP_ORIGIN ` , `API_HOST`  .
- Generate a JWT token and add it to `JWT_SECRET` .
```
openssl rand -base64 32
```
### After making sure of entering needed parameters run the playbook.
```
ansible-playbook setup.yml
```
