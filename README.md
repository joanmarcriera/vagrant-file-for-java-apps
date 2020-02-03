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
```

# How will I test your application?

So, from now onwards I will follow the instructions given in your documentation, if you need any packages that are currently not installed provide the instructions that I would need to follow.
If you read inside the Vagrantfile you will see that only maven and java have been installed, so feel free to include a line on your documentation asking for gradle to be installed if necessary. 


# UBUNTU?

If you are more used to ubuntu feel free to create a Vagrantfile with Ubuntu and include that file in your repository. 
