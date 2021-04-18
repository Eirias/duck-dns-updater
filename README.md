# Docker Duck DNS updater
This image will periodically update your [duckdns.org](https://www.duckdns.org/) DDNS

## Environment Variables
 * **DOMAIN** - the hostname to update  e.g.  test.duckdns.org
 * **TOKEN** - your authentication token from duckdns.org e.g. 1234abcd-abcd-1234-abcd-123456789abc
 * **MANUAL_IP** - (Optional) Manually set IP-address to update with
 * **INTERVAL** - (Optional) Time between updates, default = 300 seconds

## Start using .env
* Set **DOMAIN** and **TOKEN** and add **MANUAL_IP** and/or **INTERVAL** if necessary

```sh 
sudo docker run -d --env-file .env duck-dns-updater
```
