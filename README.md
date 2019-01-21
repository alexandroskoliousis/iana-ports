# iana-ports

An Awk script to process the IANA port list.

Download and save IANA's port-numbers file as `iana-port-numbers`. Then, run 
 
```shell
cat iana-port-numbers | awk -f process_iana.awk
```` 
or, in case of multiple files, run
 
```shell
awk -f process_iana.awk iana-port-numbers p2p-port-numbers
```

The script outputs two files, `tcp_port.list` and `udp_port.list`.
