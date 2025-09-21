# Zabbix NSX-T template
Zabbix template with LLD for VMware NSX 4.x

This template is designed to collect data on the status of NSX-T core components.
Please note that, depending on the size of the infrastructure and the number of objects in it, you may encounter the NSX-T API rate limit, which is set to 100 by default.
It is recommended to either use manager nodes behind a load balancer to distribute API requests or adjust the rate limiter value using the command from CLI:

```
set service http client-api-rate-limit 200
```
