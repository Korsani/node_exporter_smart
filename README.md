# About node_exporter_smart
This is a tiny perl script to gather SMART info feed prometheus textfile collector.

# Requirements

`Perl`: should be available on your system
`lsblk`: should be available on any GNU/Linux system.
`smartctl`: should be instalable via `apt install smartmontools`, `emerge smartmontools`, `pacman -S smartmontools`, ...

# Usage

`sudo node_exporter_smart <prefix> | sponge /var/lib/node_exporter/smart.prom`

`<prefix>` is the prefix of the keys. You can choose something like `node_myorg_smart`
