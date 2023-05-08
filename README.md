# 331_project
## Dependencies

### Linux Package Dependencies
* [Vagrant](https://developer.hashicorp.com/vagrant/downloads)
* [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html)

### Pip Dependencies
`pip3 install -r REQUIREMENTS.txt`

## Setup
1. Clone the repo
2. Run the following commands; this will create a folder called `resource_test` in the repo root directory
```bash
molecule init role acme.resource_test --driver-name vagrant
```
3. Copy the repo folders `molecule` and `tasks` into the newly created `resource_test` folder
```bash
cp -r molecule tasks resource_test/
```
4. Move to scenario folder: `cd resource_test`

## Execute Tests
Execute tests with the following command: `molecule test -s resource_test`
