role limited to installing krb5 client packages on ubuntu 22 and creating simple krb5.conf file

## credit

this is a gutted version of https://github.com/Turgon37/ansible-kerberos-client/tree/master

## Role Variables

| Name                                                  | Types/Values       | Description                                                                          |
| ------------------------------------------------------| -------------------|------------------------------------------------------------------------------------- |
| `kerberos_client__include_dir`                        | Path               | Directory which contains config parts to include                                     |
| `kerberos_client__include_dirs`                       | List of Path       | List of extra directory (not managed by this role) to include                        |
| `kerberos_client__keytab_principal`                   | String             | The pattern use to produce the host's principal                                      |
| `kerberos_client__realms`                             | Dict               | Dict of per realm configurations, fill the ```[realms]``` section                    |
| `kerberos_client__domains`                            | Dict               | Dict of domain-realm mapping, fill the ```[domain_realm]``` section                  |