# ansible-role-nginx-configs

This role is designed to work in conjunction with the linuxserver letsencrypt docker container. To enable a container to be made available via nginx reverse proxy put a `service_name.conf` file in `../files/nginx-confs/`. 

This role expects a dictionary of `containers` to be defined with at least the two keys `active` and `rp_enabled`. Only if both are true will the RP config be installed.