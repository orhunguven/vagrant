<h2>This is a basic Ansible-Git Automation Project</h2>
This project includes [Vagrant-Ansible-GitHub-Nginx-Supervisor-Gunicorn-Python] automation chain in general.

Thanks to this automation, you can <b>view and share changes on your flask-python application in agile way</b> without any "works on my machine" conflict.
This automation downloads necessary files, repositories and places them into the required folder structures, which created by ansible.

Ansible automation will install the packages below:

- Nginx
- Python
- Gunicorn
- Flask
- GitHub
- Supervisor


<h3>INSTALLATION</h3>

First of all, you need to have Vagrant installed on your host system. Vagrant Virtual Machine will be our guest machine.

https://www.vagrantup.com/docs/installation/

If you don't have Vagrant on your host system, please follow the link above for information and guidance about installing Vagrant.

Second, you need to have Virtualbox installed on your host system.

Go trough the given link below and download the Virtualbox which fits for your system properly.

https://www.virtualbox.org/wiki/Downloads

You need to download https://github.com/orhunguven/vagrant.git repository and store it without any change on the file hierarchy.

<h3>USAGE</h3>

1-Copy this project to the host system, which you did required installations.
2-Go to file location of the Vagrantfile on your terminal and type vagrant up.

3-vagrant up command triggers Vagrantfile, Vagrantfile triggers ansible and you will get a Virtualbox Virtual Machine which runned by vagrant and automated by ansible.
During this process, ansible will download and configure all your needs. You don't have to do anything from now on.

<h3>SEE THE RESULTS</h3>

Go to your localhost:8080 via your browser, and you will see the https://github.com/orhunguven/example.git repository is running here.

Note: If any code change happens in this repository, just apply vagrant reload --provision command at Vagrantfile location. You will get fully updated new version on your browser.
