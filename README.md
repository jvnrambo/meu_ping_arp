# meu_ping_arp
Used to check an IP with Ping and ARP for device_tracker

To Install, please create the following folder structure: /config/custom_components/meu_ping_arp and place all files there.



## Usage
Add to the code in `device_tracker.yaml` file, like a example:

```yaml
# Example configuration.yaml entry with exclude

device_tracker:
  - platform: meu_ping_arp
    count: 2
    iface: eth0
    consider_home: 60  
    interval_seconds: 20
    hosts: 
      celmotherping: 10.1.1.100
      celdaughter: 10.1.1.101
    new_device_defaults:
      track_new_devices: false

```
