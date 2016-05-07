Basic Vagrant Environment Setup
==========================

Initial configuration for a Vagrant environment running a 32-bit Ubuntu 14.04 LTS (Trusty Tahr)

### Requirements
The software below must be installed beforehand.
- Vagrant
- VirtualBox or VMWare

### Installation

After cloning this repository, run the ff. in the root directory:
```sh
vagrant up
```

Installation may take some time but after that, you can access the virtual environment via secure shell:
```sh
vagrant ssh
```

Or via the browser by following this address. [http://192.168.10.13] (http://192.168.10.13)

NOTE: If you come across write permission issues in apache, simply replace `www-data` with `vagrant` in `/etc/apache2/envvars` then restart apache

```sh
export APACHE_RUN_USER=www-data
export APACHE_RUN_GROUP=www-data
```

### Modules

The following modules will be included in the OS installation:
- PHP 5
- MySQL
- Apache2
- Redis

