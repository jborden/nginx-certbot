# Description

This was forked from https://github.com/wmnnd/nginx-certbot.git It is used as part of an Ansible playbook and setup as such, as opposed to using the original script provided.

# Vars

These are the vars to be replace by Ansible:
`__DOMAIN_NAME__` is used for the registered DNS name that points to the server this service will run on
`__DOCKER_SERVICE_NAME__` is the name of the services the WAR file run inside of

The architecture is composed of services that are also included as one large project,
   so docker-compose commands include a -p `__DOCKER_SERVICE_NAME__` option
