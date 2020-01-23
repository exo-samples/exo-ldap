# Need to use the latest version as in the previous version (2.4.40)
# the way ldap is installed avoid to run apt-get as it tries to reconfigure ldap
FROM dinkel/openldap:latest 

# Install ldap tools to help diagnosis
RUN apt-get purge -y slapd
RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -y slapd ldap-utils less
