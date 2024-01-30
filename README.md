# install-odoo9

# Postgres
```
docker run -d -e POSTGRES_USER=odoo -e POSTGRES_PASSWORD=odoo --name db9 postgres:9.4
```

# Odoo
```
docker run -p 8069:8069 --name odoo9 --link db9:db9 -t qubiq/odoo-docker:9.0
```

# Credit
```
https://hub.docker.com/r/qubiq/odoo-docker
```

```
user: admin
pasword: admin
```

