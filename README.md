WeBWorK_Vagrant
===============

vagrant files for WeBWorK development

To set up a quick dev environment for WeBWorK:

```
git clone https://github.com/whytheplatypus/WeBWorK_Vagrant.git
cd WeBWorK_Vagrant
git clone https://github.com/<your-git-username>/webwork2.git
git clone https://github.com/<your-git-username>/pg.git

#setup conf files, site.conf, webwork.apache2-config, localOverrides.conf, webwork3/environment/development.yaml

cd webwork2
vagrant up
vagrant ssh
perl -I /opt/webwork/webwork2/lib -I /opt/webwork/pg/lib /opt/webwork/webwork2/webwork3/bin/app.pl
```

Information about installing vagrant can be found here: http://docs.vagrantup.com/v2/installation/index.html

Your webwork2 folder does have to be named webwork2.
