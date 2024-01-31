# Netbox Openstack Agent 

[![Github Issues](http://img.shields.io/github/issues/SaaShup/netbox-openstack-agent)](https://github.com/SaaShup/netbox-openstack-agent/issues)
[![MIT license](http://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT)

## Description

Agent to install on a server to manage openstack though netbox.

## Settings

go to the [nodered admin page](http://localhost:1880/nodered) to change the settings.

## Clean
```
docker stop netbox-openstack-agent
docker rm netbox-openstack-agent
docker image rm saashup/netbox-openstack-agent
docker volume rm netbox-openstack-agent
```
## Build
```
docker build -t saashup/netbox-openstack-agent .
```
## Run
```
docker run -d -p 1880:1880 -v netbox-openstack-agent:/data --name netbox-openstack-agent saashup/netbox-openstack-agent 
```

Default access is *admin/saashup*

## Connect

log into [setup page](http://localhost:1880) to initialize.

# Hosting
Check https://saashup.com for more information
