## Odroid NAS/Seedbox/Adblocker

Here's my current dockerfile setup to get all of these service working together. Future plans may 
include tailscale or some other way to allow for external connections (let family/friends torrent
and or watch things)

### Dependencies
There are two additional things that are needed for this to be run

#### DuckDNS
References to duck dns should be setup to point at your own. You will also need to setup duckDNS
with a script to update its servers with the external ip of your odroid/rpi server.

#### Env file
I use VPN Unlimited and have configured Transmission OpenVPN to work with it. You'll have to set
this up for your own VPN and include credentials in an .env file for it to work

My plex instance is also setup to read the claim token from the .env file so you'll want to replace
that with your own as well

