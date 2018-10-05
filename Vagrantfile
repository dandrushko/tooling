Vagrant.configure("2") do |config|
 config.vm.define "ctl" do |ctl|
    ctl.vm.host_name = "ctl"
    ctl.vm.box = "generic/ubuntu1604"
    ctl.vm.provider "libvirt"
    ctl.vm.network "private_network", ip: "172.16.10.10",
	:libvirt__network_name => "mgmt",
	:dev => "mgmt",
	:mode => "bridge",
	:type => "bridge"
    ctl.vm.network "private_network", ip: "10.16.0.10",
	:libvirt__network_name => "public",
	:dev => "public",
	:mode => "bridge",
	:type => "bridge"

 end
 config.vm.define "cmp1" do |cmp1|
    cmp1.vm.hostname = "cmp1"
    cmp1.vm.box = "generic/ubuntu1604"
    cmp1.vm.provider "libvirt"
    cmp1.vm.network "private_network", ip: "172.16.10.20",
        :libvirt__network_name => "mgmt",
        :dev => "mgmt",
        :mode => "bridge",
        :type => "bridge"
    cmp1.vm.network "private_network", ip: "10.16.0.20",
        :libvirt__network_name => "public",
        :dev => "public",
        :mode => "bridge",
        :type => "bridge"
 end

 config.vm.define "cmp2" do |cmp2|
    cmp2.vm.hostname = "cmp2"
    cmp2.vm.box = "generic/ubuntu1604"
    cmp2.vm.provider "libvirt"
    cmp2.vm.network "private_network", ip: "172.16.10.30",
        :libvirt__network_name => "mgmt",
        :dev => "mgmt",
        :mode => "bridge",
        :type => "bridge"
    cmp2.vm.network "private_network", ip: "10.16.0.30",
        :libvirt__network_name => "public",
        :dev => "public",
        :mode => "bridge",
        :type => "bridge"
 end

end
