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

With bundled `Vagrantfile`, 

```sh
$ vagrant up
$ ansible-playbook example.yml -i example_inventry
$ ssh vagrant@127.0.0.1 -p 2222 -i ~/.vagrant.d/insecure_private_key
```

Tested OS
------------------

* Ubuntu
  * raring(13.04)

Author
------------------

Masato Hirai http://massat.github.io
