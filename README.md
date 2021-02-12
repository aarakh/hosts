# hosts
My Host Files for AdBlock,PiHole

blocked-hosts -- acts as blacklist

allowed-hosts -- acts as whitelist


Both the files can be used in popular Adblockers,PiHole

Command Line to add Whitelist in PiHole
`for I in $(curl "{https://raw.githubusercontent.com/aarakh/hosts/master/allowed-hosts}"); do pihole -w $I;done`