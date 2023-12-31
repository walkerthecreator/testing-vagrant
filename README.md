# HelloHttp Development Environment

This repository contains a Vagrant configuration for setting up a development environment for the HelloHttp web app.

## Requirements

- [Vagrant](https://www.vagrantup.com/)
- [VirtualBox](https://www.virtualbox.org/)

## Getting Started

1. Clone the HelloHttp repository:

    ```bash
    git clone https://github.com/drines-uc/hello-http.git
    ```

2. Change into the development environment directory:

    ```bash
    cd hello-http-dev-env
    ```

3. Start the Vagrant virtual machine:

    ```bash
    vagrant up
    ```

4. Access the virtual machine:

    ```bash
    vagrant ssh
    ```

## Development Workflow

- The code can be edited on the host machine and synced with the virtual machine through the `/vagrant` directory.

- Build the HelloHttp app inside the virtual machine:

    ```bash
    gcc -o /vagrant/dummyserv /vagrant/dummy_serv.c
    ```

- Run the HelloHttp app inside the virtual machine (default port is 8080):

    ```bash
    /vagrant/dummyserv 8080
    ```

## Accessing the App

Once the app is running inside the virtual machine, it can be accessed from the host machine at http://localhost:12344.





#   t e s t i n g - v a g r a n t  
 