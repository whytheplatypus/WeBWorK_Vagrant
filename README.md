WeBWorK_Vagrant
===============

vagrant files for WeBWorK development

To set up a quick dev environment for WeBWorK:

```
git clone https://github.com/whytheplatypus/WeBWorK_Vagrant.git
cd WeBWorK_Vagrant
git checkout -b packaged origin/packaged
git submodule update --init --recursive
vagrant up
```

Information about installing vagrant can be found here: http://docs.vagrantup.com/v2/installation/index.html
