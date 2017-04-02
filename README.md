# prometheus_playgroud

I set this up to automate the build out of a prometheus server with alertmanager.

It also has docker-ce docker-compose and cadvisor container running for container stats.

## Build VM

  $ vagrant up
  $ ansible-playbook -i inventory prometheus.yml

## URLs

  * *prometheus*: http://10.100.198.200:9090
  * *alertmanager*: http://10.100.198.200:9093
  * *grafana*: http://10.100.198.200:3000
