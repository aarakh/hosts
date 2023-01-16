# Description
My Host Files for AdBlock,PiHole

hosts -- acts as blacklist, this same was referenced in adlists-url at end

whitelist-url -- acts as whitelist now maintained in private repo

blacklist-url -- acts as blacklist (not in use, since using hosts file in adlists)

adlists-url -- consists of urls of other well-known block lists + my own personalized blocklist as in last line

regex-whitelist-url -- add regex of actual urls for whitelisting

regex-blacklist-url -- add regex of actual urls for blacklisting, specifying other FQDN urls in this file NOT works

Above files can be used in popular Adblockers,PiHole

pihole-updatelists.conf -- configuration file used for pihole-updatelists setup :)

### Below Whitelisting command No longer required after using https://github.com/jacklul/pihole-updatelists (thank you to jacklul)
Command Line to add Whitelist in PiHole

`for I in $(curl "{https://raw.githubusercontent.com/aarakh/hosts/master/allowed-hosts}"); do pihole -w $I;done`