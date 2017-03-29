
# Ansible Cisco Primer

More details here: https://www.linickx.com/tag/ansible

REFS:
- https://www.packetgeek.net/2016/02/kicking-the-tires-with-the-new-ansible-network-modules/
- http://www.routereflector.com/2017/02/managing-ntp-on-cisco-ios-with-ansible/
 - https://github.com/dainok/rrlabs/blob/master/ansible/ntp_config_ios.yaml
- https://github.com/brona/ansible-cisco-ios-example
- http://docs.ansible.com/ansible/ios_config_module.html
- https://docs.ansible.com/ansible/ios_command_module.html

## Show Command Testing - Credentials in File
- `show_clock.yml` - Get the time/clock, assume Priv 15, read uid/pass from file.
- `show_clock_enable.yml` - Get the time/clock, some devices require "enable"

## Show Command Testing - Prompt for Credentials
- `show_clock_prompt.yml` - Get the time/clock, assume Priv 15
- `show_clock_prompt_enable.yml` - Get the time/clock, some devices require "enable"

## Config Add
- `set_ntp.yml` - Simple adding DNS/NTP servers, assume Priv 15, read uid/pass from file.
- `set_ntp_enable.yml` - Adding DNS/NTP servers, some devices require "enable", take a backup, `wr mem`if needed

## Config Standardisation 
- standard_ntp_enable.yml - Standardise NTP and DNS i.e. add missing and remove wrong 
