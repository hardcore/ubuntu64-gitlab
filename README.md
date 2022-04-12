# Setup

Quickly set up a local Gitlab CE server using Vagrant.

### Step 1
Just run ```vagrant up``` to setup the virtual machine.
### Step 2
SSH into the virtual machine with ```vagrant ssh```.
### Gitlab ROOT password
To get the Gitlab ROOT password use `sudo  cat /etc/gitlab/initial_root_password`

# Fix VirtualBox IP range behavior
Since VirtualBox 6.1.28 only 192.168.56.0/21 IP range is allowed.

To change this behavior add for example `* 33.33.33.0/24` in /etc/vbox/networks.conf

See https://www.virtualbox.org/manual/ch06.html#network_hostonly
