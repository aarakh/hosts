# Description
My Host Files for AdBlock,PiHole

blocked-hosts -- acts as blacklist

allowed-hosts -- acts as whitelist

adlists-url -- consists of url of other well-known block lists

regex-whitelist-url --add regex of actual urls for whitelisting

regex-blacklist-url --add regex of actual urls for blacklisting, specifying other urls in this file NOT works

Both the files can be used in popular Adblockers,PiHole

## Below Whitelisting command No longer required after using https://github.com/jacklul/pihole-updatelists (thank you to jacklul)
Command Line to add Whitelist in PiHole

`for I in $(curl "{https://raw.githubusercontent.com/aarakh/hosts/master/allowed-hosts}"); do pihole -w $I;done`