# dnsmasq

> Administer dnsmasq, a lightweight DNS, DHCP, TFTP, and PXE server.
> Requires root privileges for most operations.
> More information: <https://manned.org/dnsmasq>

- Start the dnsmasq service using the default configuration:

`dnsmasq`

- Use a specific configuration file:

`dnsmasq --conf-file={{/path/to/config.conf}}`

- Run dnsmasq in the foreground for debugging:

`dnsmasq --no-daemon`

- Enable verbose logging of DNS queries:

`dnsmasq --log-queries --log-facility=-`

- Set a DHCP range with a lease duration:

`dnsmasq --dhcp-range={{192.168.0.50}},{{192.168.0.150}},{{12h}}`

- Bind dnsmasq to a specific network interface:

`dnsmasq --interface={{eth0}} --bind-interfaces`

- Display help:
`dnsmasq --help`

- Display version:

`dnsmasq --version`
