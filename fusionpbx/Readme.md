![FusionPBX Logo](logo.png)

# Minimal Alpine-based FusionPBX Image for the UDM/pro

Usage
-----

```bash
docker run -d --name fusionpbx \
	–net=host \
	-v /etc/localtime:/etc/localtime:ro \
	-v /mnt/data/fusionpbx:/data \
	-e PGPASSWORD=${postgres_pass} \
	tusc/fusionpbx-freeswitch 
```
Access FusionPBX through: 
```
http://your-ip-here
```


