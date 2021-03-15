# ansible

## Step-1: Introduction to ansible


## Install vim using command-line

```
ansible -m yum -a "name=vim state=latest"  console --become
```

## UnInstall vim using command-line

```
ansible -m yum -a "name=vim state=absent"  console --become
```

where:
1. "ansible"        ---> command module ( /bin/ansible ) 
2. "-m"             ---> module (i.e which module you want to import)
3. "yum"            ---> module name 
4. "-a"             ---> module argument
5. "name=vim"       ---> package name (vim editor)
6. "state=present"  ---> means it shoudl install. State values can only be
                         ( absent, installed, latest, present, removed, got: lst)
7. "console"        ---> group / vm Name provided in inventry file
8. "--become"       ---> becomes sudo user