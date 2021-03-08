# junos-command

## JuneOS
```
Show Mode
Show vlan
Show route
Show ofpf
Show ofpf interface
Show ofpf route
Show interface fe-1/1/1 ?
Show interface ge-0/0/2
Show interface ge-0/0/0.0 brief
Show interface ge-0/0/2 terse
Show interface ge-0/0/2.0 terse
Show interface terse
Show interface terse | ?
Show interface terse | match
Show interface terse | count
Show interface brief
show | compare
Show | compare rollback 1
show | compare rollback 2
show configuration | display set | match ge-0/0/0
show configuration | display omit
show group mygroup
run show interface
run show system users
configure exclusive
run request system logout terminal pts/1
```
## Monitor
```
monitor interface traffic matching
monitor interface ge-0/0/0
run monitor interface ge-0/0/0
```


## Configuration Mode
```
configure
set protocols
set firewall
set system host-name <name>
edit interface
edit ge-0/0/0
show
up
exit
run show bgp sumary
configure private <— config private
configure exclusive <—- none access
set system syslog file messages any notice
```

## Delete
```
delete interfaces ge-0/0/0 unit 0 family init
```

## Rollback command
```
rollback
rollback 0
rollback 1 <<— use config lasted
show | compare rollback 2
```

## Commit
```
commit check
mike@juniper# commit confiremd 
mike@juniper# commit 
```
## Deactivate
```
deactivate bgp
deactivate interface ge-0/0/2
```
## Activate
```
activate bpg
```
## Load
```
load ?
load merge ?
load merge /var/tmp/test.conf
```
## Vlan 
```
set vlans employee-vlan
set vlans employee-vlan vlan-id 100
set interfaces ge-0/0/1 unit 0 family ethernet-switching vlan members employee-vlan 
set interfaces ge-0/0/2 unit 0 family ethernet-switching vlan members employee-vlan 
set interfaces ge-0/0/3 unit 0 family ethernet-switching vlan members employee-vlan 
```
## Firewall
```
set firewall
```
## Authe

## Log
```

```
## Juniper solution
```

```
## Tools
1. saltstack
2. Netconf <— connectivity template use grpc over ssh only 
3. Openconfig <— configuration and delete 
	3.1 Vendeor-netual
	3.2 streaming telemetry
  3.3 yang <— data models
	3.4 common data models

### LABS
```
https://jlabs.juniper.net/vlabs/portal/index.page
```
