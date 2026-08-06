# SiberKapan Blocklist

Real-time threat intelligence blocklist, auto-updated every 6 hours from
[siberkapan.org](https://siberkapan.org) — sourced exclusively from our own
sensor network (honeypots, FortiGate webhooks, nginx watchers), not
third-party aggregation.

## Lists

| File | Description |
|---|---|
| `lists/all-feed.txt` | Combined FortiGate + Honeypot + nginx sources |
| `lists/high-confidence.txt` | Score ≥75 only |
| `lists/fortigate-feed.txt` | FortiGate-sourced only |
| `lists/honeypot-feed.txt` | Honeypot-sourced only |
| `lists/nginx-feed.txt` | nginx watcher-sourced only |
| `lists/suricata.rules` | Suricata ruleset format |
| `lists/wazuh-cdb.txt` | Wazuh CDB list format |

## Usage

curl -s https://raw.githubusercontent.com/<user>/siberkapan-list/main/lists/all-feed.txt

## Contributing

Feed/sensor contributors: see [siberkapan.org/contributors](https://siberkapan.org/contributors)

## Also part of the SiberKapan ecosystem

- Main platform: https://siberkapan.org
- MISP feed: https://siberkapan.org/misp-feed/
