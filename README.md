# resolver

Resolver is designed to repeatedly check the resolv.conf file on linux machines to ensure that the data contained within is correct.

on first run, you will be prompted to add primary and secondary DNS server addresses. resolver will then generate a new resolv.conf
in the /etc/ directory overwriting the default one, then while resolver is running, it will monitor this file and regenerate if it
is overwritten

resolver is a node application and must be run as root.

sudo node /path/to/repo/resolver/resolver
