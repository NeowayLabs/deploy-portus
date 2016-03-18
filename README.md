Deploy Portus
===

## Things to change

You should change a few environment vars on the `environment.sh` section:

 - `PORTUS_SECRET_KEY_BASE`: should be generate by a `rake secret` command
 - `PORTUS_EMAIL_SMTP_PASSWORD`: should be the password for email
 - Everywhere it says `your-registry`

Also, all domain names should point to your FQDN, so change your-registry.com.br to your FQDN.

The certificates written in the `haproxy-config.sh` section are fake and should be replaced by a valid key and certificate authorized by a CA.
