WeBWorK_Vagrant
===============

vagrant files for WeBWorK development

To set up a quick dev environment for WeBWorK:

```
git clone https://github.com/whytheplatypus/WeBWorK_Vagrant.git
cd WeBWorK_Vagrant
git submodule init
git submodule update
cd webwork2
vagrant up
```

Information about installing vagrant can be found here: http://docs.vagrantup.com/v2/installation/index.html

To set up with you own dev repo:

```
git clone https://github.com/whytheplatypus/WeBWorK_Vagrant.git
cd WeBWorK_Vagrant
git checkout clean
git submodule add <your webwork2 url>
```

Your webwork2 folder does have to be named webwork2.
