# go-pihole-stats

WIP

Get stats from your Pi-hole instance at the command-line.

To use, one must have a running Pi-hole instance on one's network. Export the following environment variables:

Note: the auth token is stored in the `WEBPASSWORD` variable in `/etc/pihole/setupVars.conf` on the Pi-hole machine.

```bash
export PIHOLE_URL="http://pi.hole/admin"
export PIHOLE_AUTH="auth token"
```

Install the program:

```bash
go get -v git.envs.net/hyperreal/go-pihole-stats
```

Ensure GOPATH is set and in PATH:

```bash
export GOPATH="${HOME}/go"
export PATH="${PATH}:${GOPATH}"
```

Run the command to get Pihole stats:

```bash
go-pihole-stats
```
