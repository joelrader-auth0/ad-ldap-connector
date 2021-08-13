# ad-ldap-connector
Repo for documentation and code to enable the deployment of an AD-LDAP connector for an Auth0 tenant.
---
# Getting Started
To get started you will need an Auth0 tenant that you wish to add an LDAP connection to. Once logged into your tenant, perform the following actions to create a new LDAP connection:
1. Navigate to **Authentication** > **Enterprise**
2. Create a new **Active Directory / LDAP** connection
3. Provide a **Connection Name** just using alphanumeric values and a hyphen (e.g. `This-is-a-test-LDAP-connection`)
4. Enter a **Display Name** as you'd like to have it shown on the Universal Login page
5. Optionally enter in a **Logo URL**
6. For now, turn on the `Disable Cache` option to force the LDAP connector to query the LDAP server on every request to simplify troubleshooting
7. Click **Create**
8. Copy the **Provisioning Ticket URL** that is shown, as you will need it to update the LDAP connector startup environment variables.
9. Under the **Applications** tab, enable the LDAP connector for at least one application.
10. Back on the **Active Directory / LDAP** connector screen, you will see the new LDAP connection listed. Until the LDAP connector has been started, the connection will show as `offline`.
![LDAP Connections](/img/ldap-connections.png?raw=true "LDAP Connections")
---
