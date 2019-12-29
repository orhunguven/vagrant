This project includes [Vagrant-Ansible-GitHub-Nginx-Supervisor-Gunicorn-Python] chain in general.


Ansible provision will install the packages below:

- Nginx
- Python
- Gunicorn
- Flask
- GitHub
- Supervisor

This automation also downloads necessary files, repositories and places them into the required folder structures which created by ansible.

Vagrant project directory tree shown below:

.
├── provision
│   ├── site.yml
│   └── templates
│       ├── nginx_config.jinja2
│       └── supervisor_config
└── Vagrantfile

2 directories, 4 files
----------------------

First of all, you need to have Vagrant installed on your host system. Vagrant Virtual Machine will be our guest machine.

https://www.vagrantup.com/docs/installation/
If you don't have Vagrant on your host system, please follow the link above for information and guidance about installing Vagrant.

Second, you need to have Virtualbox installed on your host system.

https://www.virtualbox.org/wiki/Downloads
Go trough given link and download the Virtualbox which fits for your system properly.

https://github.com/orhunguven/vagrant.git repository tree shared above. You need to get this repository without change the file hierarchy.

Usage:

Copy this project to a desired host system, which you installed Vagrant at previous stage.
Go to file location of the Vagrantfile on your terminal and type vagrant up.

vagrant up command triggers Vagrantfile, Vagrantfile triggers ansible and you will get a Virtualbox Virtual Machine which runned by vagrant and automated by ansible.
During this process, ansible will download and configure all your needs. You don't have to do anything.

Go to your localhost:8080 via your browser, and you will see the https://github.com/orhunguven/example.git repository is running here.
If any code change happens in this repository, just apply vagrant reload --provision command. You'll get fully updated new version on your browser.
