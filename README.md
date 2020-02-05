# Wordpress in Docker Generator

Easily spin up a new Wordpress instance and database in Docker containers. Taken from the example given by Docker.

Taken and modified from the quickstart by [docker][1].

Great for running on AWS EC2 instances.

Be sure to setup an image snapshot (storage system snapshot) and an instance template (using the storage snapshot) that has `docker` and/or `git` (to pull this repo, or you can rsync from your current machine to the EC2 startup host) and any other packages you want/need. Then save the snapshot, set the instance, spindown the server. Spin up a new one from the template to confirm everything is working.

Be sure to setup elastic IP's for the container, then route a domain or subdomain from your host provider with an 'A record' to the IP.

[1]: https://docs.docker.com/compose/wordpress/

> Created by [Spencer Pollock](https://github.com/srepollock) 2020
