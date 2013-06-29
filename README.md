WeBWorK_Vagrant
===============

vagrant files for WeBWorK development

To set up a quick dev environment for WeBWorK:

```
git clone https://github.com/whytheplatypus/WeBWorK_Vagrant.git
cd WeBWorK_Vagrant
git submodule update --init --recursive
vagrant up
```

Information about installing vagrant can be found here: http://docs.vagrantup.com/v2/installation/index.html

To set up with you own dev repo:

```
git clone https://github.com/whytheplatypus/WeBWorK_Vagrant.git
cd WeBWorK_Vagrant
```
Then edit the `.gitmodules` file so that the urls point to the pg and webwork2 repos you want.
To finish up run:
```
git submodule update --init --recursive
vagrant up
```


Your webwork2 and pg folders do have to be named webwork2 and pg respectively.
