Vagrant.configure("2") do |config|
  config.vm.box = "alpine/alpine64"
  config.vm.box = "alainvanhoof/alpine-virtual-x86_64-3.8"
  config.vm.provision :shell, path: "bootstrap.sh"


config.vm.provider "virtualbox" do |vb|

	
vb.customize ["modifyvm", :id, "--usb", "on"]
vb.customize ['usbfilter', 'add', '0', '--target', :id, '--name', 'ASIX Elec. Corp. AX88179 [0100]', '--vendorid', '0b95', '--productid', '1790']
end
end
