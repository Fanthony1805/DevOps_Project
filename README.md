# ECE_DevOps_Project
Project DevOps made by Anthony FERREYROLLES and Nassim GHANEM

# User API http-server

Simple http-server with a user API

##  TODO

* Clone this repo and using [duplicating](https://help.github.com/en/github/creating-cloning-and-archiving-repositories/duplicating-a-repository) create your own repository on GitHub or GitLab
* **Important!** Make your repository **PRIVATE**
* Find all the TODO comments and enrich this app
* If you have questions, ask me by email sergei@adaltas.com (link your private repo, if you have technical questions and invite me to you project)

## Functionality

* Uses default configuration with a path of the file storage
* Start http-server
* Use Vagrant with Shell Provisioner
* Install GitLab using Vagrant and Ansible Provisioner
* Use prepared User API application and run tests
* Use Travis CI and Heroku for the tests and CI/CD
* Use Docker Hub
* (Use Istio)

## Tools

Travis CI -
https://travis-ci.com/github/Fanthony1805/ece-devops-project

Heroku -
https://dashboard.heroku.com/apps/module5-devops

Docker Hub -
https://hub.docker.com/repository/docker/fanthome18/devops_project_ferreyrolles_ghanem?ref=login






## Installation

```
git clone ...
npm install
```

## Usage

```
npm start
```

Go to `http://localhost:3000`


## Using Vagrant with Shell Provisioner

Move to assets/part-1.

Launch Vagrant :

```
vagrant up
```

Check its status :

```
vagrant status
```

Check that everything is ok by connecting to the VM via SSH :

```
vagrant ssh centos_server
```

Start provisioning :

```
vagrant provision
```


## GitLab installation using Vagrant and Ansible Provisioner

Move to assets/part-2.

Launch Vagrant :

```
vagrant up
```

Check its status :

Go to `http://20.20.20.2`

Choose a password and login as root :

```
vagrant ssh centos_server
```

Update the playbooks on the VM :

```
vagrant upload playbooks /vagrant/playbooks gitlab_server
```

Start provisioning :

```
vagrant provision
```

## Use prepared User API application and run tests

Install application:

```
npm install
```

Run tests:

```
npm test
```

Start application:

```
npm start
```

## Comments

We did the part on Istio but the code was too heavy and we couldn't manage to integrate it to the project :(
