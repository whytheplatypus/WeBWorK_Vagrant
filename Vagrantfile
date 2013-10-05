Vagrant.configure("2") do |config|
    config.vm.define :webwork do |ww_config|
        ww_config.vm.box = "webwork"
        ww_config.vm.box_url = "https://dl.dropboxusercontent.com/u/3154638/webwork.box"
        ww_config.vm.provision :shell, :path => "bootstrap.sh"
        ww_config.ssh.max_tries = 10
        config.vm.network :forwarded_port, guest: 80, host: 8888
        config.vm.network :forwarded_port, guest: 3306, host: 8889
        config.vm.network :forwarded_port, guest: 5432, host: 5433
        config.vm.network :forwarded_port, guest: 3000, host: 3000
	ww_config.vm.hostname = "WeBWorK"
        ww_config.vm.synced_folder "webwork2", "/opt/webwork/webwork2",  :extra => 'dmode=777,fmode=777'
        ww_config.vm.synced_folder "pg", "/opt/webwork/pg",  :extra => 'dmode=777,fmode=777'
    end
end
