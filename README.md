# iana-ports

An Awk script to process the IANA port list.

Download and save IANA's port-numbers file as `filename`. Then, run 
 
```shell
cat [filename] | awk -f process_iana.awk
```` 
or, in case of multiple files, run
 
```shell
awk -f process_iana.awk [filename #1] ... [filename #n]
```

The script outputs two files, `tcp_port.list` and `udp_port.list`.
