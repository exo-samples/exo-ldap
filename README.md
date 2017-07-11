# exo-ldap
Example of eXo platform using ldap

## Ldap

### Only start ldap

```
docker-compose up ldap
```

### Reset data

```
docker-compose down -v
```

### List content

```
docker-compose exec ldap slapcat
```

### Connect to the ldap

You can use [JXplorer](http://www.jxplorer.org/) to update or browse the ldap content

With the default configuration declared on the project, you can use this credentials to connect to the ldap :

| DN | Password | Role |
|----|----------|------|
| cn=admin,dc=exo-samples,dc=org| password | Administrator |
| cn=root,ou=users,dc=exo-samples,dc=org | gtn | Read only |
| cn=test1,ou=users,dc=exo-samples,dc=org | gtn | Read only |

Example of connection as admin in jxplorer : ![Connection][doc/jxplorer_admin_connection.png]
