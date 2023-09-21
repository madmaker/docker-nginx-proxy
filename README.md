# Docker nginx proxy

1. check docker-compose.yml
2. check conf.d/default.conf
3. copy conf.d/site.conf.template to *yoursite*.conf:
   `cp conf.d/site.conf.template yoursite.conf`
4. edit yoursite.conf:
   5. Change CHANGE_TO_DOMAIN_NAME, ex. google.com
   6. Change CHANGE_TO_TARGET_HOST_AND_PORT$, ex. mycomp.com
7. Run service with command `make up`

Run `make down` to stop service

Run `make sh` to enter to nginx container

### Path of nginx inside container:

- /etc/nginx