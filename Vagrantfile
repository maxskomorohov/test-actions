Vagrant.configure("2") do |config|

  # =========================
  # GIT Lab Actions
  # =========================
  config.vm.define "github-actions" do |jenkins|
    jenkins.vm.box = "bento/ubuntu-24.04"
    jenkins.vm.hostname = "github-actions"
    jenkins.vm.provider "virtualbox" do |vm|
      vm.name = "github-actions"
      vm.memory = 2048
      vm.cpus = 4
    end

    jenkins.vm.network "public_network", bridge: "en0: Wi-Fi"

#     jenkins.vm.provision "shell", inline: <<-SHELL
#       apt-get update
#     SHELL
  end

end