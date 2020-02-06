# vagrant-file-for-java-apps



This Vagrant file has been created using [ centos7 ](https://app.vagrantup.com/centos/boxes/7) as template .


1) You will need virtualbox installed on your computer.
2) Clone this repository on your computer
```bash
$ git clone https://github.com/joanmarcriera/vagrant-file-for-java-apps
```
3) Run ` vagrant up` .
```bash
$ cd vagrant-file-for-java-apps
$ vagrant up
```


Inside the Vagrant file you can see that port 8080 of your machine will provide access to port 80 inside the Vagrant running OS, if that port is already used on your machine feel free to use any other port by changing the Vagrant file and running `vagrant destroy` before running `vagrant up` again. 


# How to test if the environment is configured correctly.

After `vagrant up` you should be able to `vagrant ssh` 

```bash

✔ ~/my_repos/vagrant-file-for-java-apps [master|✚ 1…11]
12:36 $ vagrant ssh
[vagrant@localhost ~]$ sudo su -
Last login: DATE REDACTED
[root@localhost ~]$
```

# How will your application be tested ?

So, from now onwards we will follow the instructions given in your documentation, if you need any packages that are currently not installed provide the instructions that we need to follow.

If you read inside the Vagrantfile you will see that only maven and java have been installed, that does not mean that you have to use them, but if you use something else you should include a line on your documentation asking for gradle(or any other dependency) to be installed and configured.


# UBUNTU?

If you are more used to ubuntu feel free to create a Vagrantfile with Ubuntu and include that file in your repository, or link the repository with the Vagrantfile for us to use. 
