ansible-motd-dq2
================

An ansible role to edit motd to show pixel arts of DQ2 characters.

The Original idea is [here](http://qiita.com/makocchi/items/5549c41526d6a6cabab1) .

Role Variables
--------------

`motd_dq2_figure` specifies the character to show.
Available values is listed below.

* slime (default)
* slime-beth
* metal-slime
* bubble-slime
* hagure-metal
* slime-allstar
* dq2-lorasia
* dq2-samaltria
* dq2-moonbrooke
* dq2-allstar
* dq2-allstar_half

Example
-------------------------

### Install from galaxy.ansible.com

Install with

```sh
$ ansible-galaxy install massat.ansible-motd-dq2
```

and write playbook

```yml
- hosts: example
  roles:
  - { role: massat.ansible-motd-dq2, motd_dq2_figure: slime-beth }
```

then, run role.

```sh
$ ansible-playbook example.yml -i path/to/your-inventry
```

### Download from GitHub

Vagrantfile is bundled in repositry.
So, clone with

```sh
$ git clone git@github.com:massat/ansible-motd-dq2.git
$ cd ansible-motd-dq2
```

and vagrant up, and run playbook.

```sh
$ vagrant up
$ ansible-playbook example.yml -i example_inventry
```

You can see it on ssh login.

```sh
$ ssh vagrant@127.0.0.1 -p 2222 -i ~/.vagrant.d/insecure_private_key
```

Tested OS
------------------

* Ubuntu
  * raring(13.04)

Author
------------------

Masato Hirai http://massat.github.io
