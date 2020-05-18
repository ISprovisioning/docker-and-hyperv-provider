ENV['VAGRANT_DEFAULT_PROVIDER'] = 'docker'
 
Vagrant.configure("2") do |config|
 
config.vm.define "my-little-container" do |m|
 
m.vm.provider :docker do |d|
d.name = 'my-little-container'
d.build_dir = "."
d.cmd = ["ping", "-c 51", "127.0.0.1"]
d.remains_running = true
d.vagrant_machine = "dockerhostvm"
d.vagrant_vagrantfile = "./DockerHostVagrantfile"
end
end
end