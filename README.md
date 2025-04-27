# 42Cursus - Cloud-1

## Automated deployment of the [Inception](https://github.com/lxup/42Cursus-inception) project


To set up the project, follow these steps:
1. Clone the repository:
```bash
git clone https://github.com/lxup/42Cursus-cloud-1
cd 42Cursus-cloud-1
```
2. Edit the `hosts` file to add your server's IP address:
```bash
nano ./hosts
```
3. Edit the `ansible.cfg` file to set your `roles_path`:
```bash
nano ./ansible.cfg
```
4. Install the required dependencies:
```bash
ansible-playbook -i hosts playbooks/install-dependencies.yml
```
5. Run the playbook to deploy the Inception project:
```bash
ansible-playbook -i hosts playbooks/deploy.yml
```