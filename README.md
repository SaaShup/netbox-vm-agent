# Netbox VM Agent 

[![Github Issues](http://img.shields.io/github/issues/SaaShup/netbox-vm-agent)](https://github.com/SaaShup/netbox-vm-agent/issues)
[![MIT license](http://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT)

## Description

Agent to install on a server to manage vm though netbox.

## Settings

go to the [nodered admin page](http://localhost:1880/nodered) to change the settings.

## Clean
```
docker stop netbox-vm-agent
docker rm netbox-vm-agent
docker image rm saashup/netbox-vm-agent
docker volume rm netbox-vm-agent
```
## Build
```
docker build -t saashup/netbox-vm-agent .
```
## Run
```
docker run -d -p 1880:1880 -v netbox-vm-agent:/data --name netbox-vm-agent saashup/netbox-vm-agent 
```

Default access is *admin/saashup*

## Contribute

### Run locally

On the root of the project run:

```
npm install
npx node-red -u . -s settings_dev.js
```

Then you can browse http://localhost:1880/nodered. Default access is *admin/saashup*.

## Connect

log into [ui page](http://localhost:1880) to see your docker assets

## Connect

log into [setup page](http://localhost:1880) to initialize.

# Hosting
Check https://saashup.com for more information
