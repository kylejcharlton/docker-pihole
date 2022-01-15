## docker-pihole

This is my personal docker setup for Pi-Hole which uses cloudflared as an upstream resolver. Since this uses Docker
Compose, you do not need to depend on a fork of pihole to implement this functionality with the posibility of being
behind on any updates.

I intend to add front facing DoH and DoT server functionality with the help of a reverse proxy and a DNS proxy to
funnel queries directly to Pi-Hole so that it can be accessable outside of your own network. This will require having
a domain you own through either a DDNS service or through a registrar along with a way to generate and renew
certificates to use for HTTPS and TLS.

See the respective repositories for additional configuration:

- [pihole/pihole](https://github.com/pi-hole/docker-pi-hole)
- [visibilityspots/cloudflared](https://github.com/visibilityspots/dockerfile-cloudflared)
