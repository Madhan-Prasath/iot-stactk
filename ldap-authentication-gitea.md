## Authentication Type: LDAP (via BindDN)

### Configuration Details:

- **Host:** example-host
- **Port:** 389
- **Bind DN:** CN=gitea gitea,CN=Users,DC=techplayr,DC=com
- **User Search Base:** DC=test,DC=com
- **User Filter:** (sAMAccountName=%s)
- **Email Attribute:** mail

### Step-by-Step Integration Guide:

1. **Introduction:**
    
    - LDAP authentication is configured in Gitea to allow users to authenticate against an LDAP server.
2. **Prerequisites:**
    
    - Ensure you have administrative access to Gitea and the LDAP server.
    - Gather the LDAP server details: Host, Port, Bind DN, User Search Base, User Filter, and Email Attribute.
    - 
1. **Configuration in Gitea:**
    
    - Login to Gitea as an administrator.
    - Navigate to **Site Administration > Authentication Sources**.
4. **Add Authentication Source:**
    
    - Click on **Add Source**.
    - Choose **LDAP** as the authentication type.
5. **LDAP Configuration:**
    
    - Provide the following details:
        - **Host:** example-host-name
        - **Port:** 389
        - **Bind DN:** CN=gitea gitea,CN=Users,DC=test,DC=com
        - **User Search Base:** DC=test,DC=com
        - **User Filter:** (sAMAccountName=%s)
        - **Email Attribute:** mail
    - Save the configuration.
6. **Testing the Integration:**
    
    - Attempt to log in with an LDAP user account to verify the integration.
    - Check Gitea logs for any authentication-related errors.
7. **Troubleshooting:**
    
    - If authentication fails, refer to the [official documentation](https://www.youtube.com/watch?v=EacpMaIQYhg) or review the logs for error messages.
    - Ensure that the LDAP server is reachable from the Gitea server.
8. **Conclusion:**
    
    - LDAP authentication is now configured for Gitea. Ensure to communicate the changes to the relevant stakeholders.

## Additional Resources:

- [LDAP Authentication Documentation](https://www.youtube.com/watch?v=EacpMaIQYhg)
- [Anonymous Access to Active Directory](https://activedirectoryfaq.com/2016/09/anonymous-access/)
- [Gitea LDAP](https://www.youtube.com/watch?v=EacpMaIQYhg)