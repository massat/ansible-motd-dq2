ansible-motd-dq2
================

An ansible playbook to edit motd to show pixel arts of DQ2 characters.

The Original idea is [here](http://qiita.com/makocchi/items/5549c41526d6a6cabab1) .

## Get started

With bundled Vagrantfile,

```sh
$ vagrant up
$ ansible-playbook playbook.yml -i vagrant_inventry
$ ssh vagrant@127.0.0.1 -p 2222 -i ~/.vagrant.d/insecure_private_key
```

## Availeble figures

* slime           
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

Figures are specified with a variable `figure`, and default figure is `slime`.

Lorasia comes with,

```sh
$ ansible-playbook playbook.yml -i vagrant_inventry --extra-vars "figure=dq2-lorasia"
```

## Supported OS

* ubuntu(only 13.04 tested)
