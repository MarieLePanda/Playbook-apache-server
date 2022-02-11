# Playbook-Apache-server

Playbook-Apache-server is an ansible playbook to install Apache service on ubuntu.

## Installation

Download directly the playbook from this Git repository

```bash
githttps://github.com/MarieLePanda/Playbook-apache-server.git
cd Playbook-Apache-server
```

## Configure

The file default.yml in the vars folder contains the variable to set for your WordPress installation.
It contains:
- app_user: a remote non-root user on the Ansible host that will own the application files.
- http_host: The domain name.
- `http_conf`: the name of the configuration file that will be created within Apache.
- `http_port`: HTTP port, default is 80.
- `disable_default`: whether or not to disable the default Apache website. When set to true, your new virtualhost should be used as the default website. Default is true.

## Run

To run the playbook
```Bash
ansible-playbook playbook.yml
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.



## License
[Apache License 2.0](http://www.apache.org/licenses/LICENSE-2.0)
