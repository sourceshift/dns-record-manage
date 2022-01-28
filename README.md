# Make DNS Entry

Make a DNS entry. (GoDaddy)

## Arguments

- `--domain`: Domain to create DNS entry for. Defaults to `sourceshift.org`.
- `--ttl`: TTL for DNS entry. Defaults to `600`.
- `--authtoken`: Enter Provider Token, For multiple tokens add them in comma separated format.
- `--record`: Domain hostname to create DNS entry for.
- `--points`: IP address to point to.

## How to run

```bash
wget https://raw.githubusercontent.com/sourceshift/dns-controller/main/add-a-record
chmod +x add-a-record
./add-a-record \
    --authtoken "$GODADDY_KEY:$GODADDY_SECRET" \
    --record=cool.application \
    --points=127.0.0.1
```
