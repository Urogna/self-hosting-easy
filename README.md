# self-hosting-easy

Quick and easy docker compose set up for self hosting with support for sso protected services

## Setup

Follow instructions in each file (replace secrets, domains, etc) so that this setup works for you.
This repo servse to give an easy guidline to setup a minimal self hosting system with SSO protection (google auth, Auth0, Azure AD, etc).

## Don't forget

To be reachable from outside of your private network, you'll need to forward ports 80 and 443 from your router to the SERVER_IP to port 80 and 443 respectively (to where our caddy instance is running).
You'll also need a domain you own 'example.com' and a DDNS service (I use DuckDNS) that points to your public IP

## Start

Install and setup docker with its compose plugin (refer to [Docker installation documentation](https://docs.docker.com/compose/install/linux/#install-using-the-repository))

then run:

```
docker compose up -d
```
