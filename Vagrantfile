Vagrant.configure(2) do |config|

  # all hosts built on centos 6
  config.vm.box = "bento/centos-6.7"
  config.ssh.insert_key = "true"

  # provisioning
  config.vm.provision :ansible do |ansible|
    ansible.playbook = "playbook.yml"
    ansible.sudo = true
    ansible.raw_arguments = "--step"
  end
end
