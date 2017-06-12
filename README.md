# prometheus_playgroud

I set this up to automate the build out of a prometheus server with alertmanager.

It also has docker-ce docker-compose and cadvisor container running for container stats.

## Dependencies

This has only been tested on OSX. I used homebrew to install ansible.

  * vagrant
  * virtual box
  * ansible - `brew install ansible`

## Build VM

  $ `vagrant up`

## URLs

  * *prometheus*: http://localhost:9090
  * *alertmanager*: http://localhost:9093/alert-manager/
  * *grafana*: http://localhost:3000

## updates

I changed from using a virtual box private network to using port forwarding. My VPN software was making using the private network unsustainable.
