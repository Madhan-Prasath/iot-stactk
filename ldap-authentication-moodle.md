# Configuring Moodle LDAP using Windows Active Directory

## Accessing LDAP Server Settings

1. Navigate to Site administration > Plugins.
2. In the Authentication area, select Manage authentication.
3. Access the LDAP server settings.

## Server Configuration

Host: ldap://ip-address-or-url

(Leave other fields as default)

## Bind Settings

- Prevent password caching: Yes
- Distinguished name: CN=example-name,CN=Users,DC=example,DC=com
- Password: password

## User Lookup Settings

- User type: MS ActiveDirectory
- Contexts: dc=example,dc=com
- Search subcontexts: Yes
- Dereference aliases: No
- User attribute: samaccountname

## Data Mapping

- First name: givenName
- Last name: sn
- Email address: mail

Click on the Save changes button to finish the configuration.

## Enabling LDAP Authentication

1. Return to Site administration > Plugins.
2. Click the eye icon to enable the LDAP authentication.

## Reference

- [Moodle LDAP using windows AD](https://techexpert.tips/moodle/moodle-ldap-authentication-active-directory/)
- [Moodle official documentation](https://docs.moodle.org/403/en/LDAP_authentication)