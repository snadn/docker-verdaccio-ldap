# docker-verdaccio-ldap

## GUIDE

1. config `docker-compose.yml` such as:

```yml
verdaccio-ldap:
    image: snadn/verdaccio-ldap
    ports:
        - "4873:4873"
    volumes:
        - /srv/verdaccio-ldap/storage:/app/storage
        - /srv/verdaccio-ldap/config:/app/config
    restart: always
```

2. start the service `docker-compose up -d verdaccio-ldap`
