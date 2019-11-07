## LDAP

- http://localhost:389
- http://localhost:8080

```bash
perl script/csv2ldif2-1.1/csv2ldif2.pl -b dc=example,dc=org < resource/MOCK_DATA.csv > resource/mock_data.ldif
ldapmodify -h localhost -D "cn=admin,dc=example,dc=org" -w admin -p 10389 -a -f resource/mock_data.ldif
```

## Config

- [images/Screenshot_2019-11-07 Keycloak Admin Console.png](images/Screenshot_2019-11-07 Keycloak Admin Console.png)

## Resource

- https://idaccessman.wordpress.com/2018/08/26/ldap-federation-with-keycloak