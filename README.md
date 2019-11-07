# Gemelnet  

Gemelnet is a fork from [Containernet](https://containernet.github.io) which itself is a fork of Mininet that uses Docker instead of LXC. Our main modification is allowing multi-interface hosts (simulating a public and private interface).

# Motivation

In ATMoS, in each VN there are gateway hosts (that run Snort). We want them to have a public and private interface for the sake of more resemblance to a real-work set-up.

# Installation

The installation is exactly same as Containernet:

```
$ sudo apt-get install ansible git aptitude
$ git clone https://github.com/blackvvine/gemelnet
$ cd containernet/ansible
$ sudo ansible-playbook -i "localhost," -c local install.yml
$ cd ..
$ sudo python setup.py install
```

For more info, visit the [Containernet](https://github.com/containernet/containernet) repo.


