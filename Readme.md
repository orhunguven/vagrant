This project includes [Vagrant-Ansible-GitHub-Nginx-Supervisor-Gunicorn-Python] chain in general.


Ansible automation will install the packages below:

- Nginx
- Python
- Gunicorn
- Flask
- GitHub
- Supervisor

This automation also downloads necessary files, repositories and places them into the required folder structures which created by ansible.

INSTALLATION

First of all, you need to have Vagrant installed on your host system. Vagrant Virtual Machine will be our guest machine.

https://www.vagrantup.com/docs/installation/

If you don't have Vagrant on your host system, please follow the link above for information and guidance about installing Vagrant.

Second, you need to have Virtualbox installed on your host system.

Go trough the given link below and download the Virtualbox which fits for your system properly.

https://www.virtualbox.org/wiki/Downloads

You need to get https://github.com/orhunguven/vagrant.git repository without change the file hierarchy.

USAGE

1-Copy this project to the host system, which you did required installations.
2-Go to file location of the Vagrantfile on your terminal and type vagrant up.

3-vagrant up command triggers Vagrantfile, Vagrantfile triggers ansible and you will get a Virtualbox Virtual Machine which runned by vagrant and automated by ansible.
During this process, ansible will download and configure all your needs. You don't have to do anything from now on.

SEE THE RESULTS

Go to your localhost:8080 via your browser, and you will see the https://github.com/orhunguven/example.git repository is running here.

Note: If any code change happens in this repository, just apply vagrant reload --provision command at Vagrantfile location. You will get fully updated new version on your browser.
