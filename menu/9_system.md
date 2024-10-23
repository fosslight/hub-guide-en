---
sort: 9
published: true
---
# System
```note
(Admin Only) Check the FOSSLight Hub log or change the operation data.
```

## Code Management
![config](images/9_system_code.png)
- Set the configuration values to be loaded during system operation.

## User Management
![config](images/9_system_user.png)
Check the list of registered accounts and update the information.
- **Create button** : Creates a Token to be used for the [Rest API](../advanced/2_rest_api.md).
- **Reset button** : Resets the password to the same ID as the ID.
- **Use YN** : Sets up dormant account.
- **Admin** : Admin authority is granted.

## History List
![config](images/9_system_history.png)
Check the data changes in the DB.

## Notification
Manage the notification pop-up displayed when users access the system.
### ![config](images/9_system_noti_list.PNG)
Check and edit the list of previously registered notifications.

### ![config](images/9_system_noti_add.PNG)

Click the '+' button at the bottom left of the list to add a notice.
- Start Date : Notification start date
- End Date : Notification end date
- Publish : If checked, a notification pop-up is displayed.

## Sent Mail List
![config](images/9_system_mail.png)
Check the mail delivery history.

## Vulnerability Log
![config](images/9_system_vul.png)
Check for Vulnerability Data changes.


## Server Setting
![config](images/9_system_server.png)
### Authentication using LDAP
FOSSLight Hub supports user password authentication using LDAP in environments where LDAP, such as Active Directory, can be used via JNDI.
- Provider Url: Set the LDAP server information in the format ldap://&lt;AD_SERVER_IP&gt;:&lt;LDAP_PORT&gt;. (javax.naming.Context.PROVIDER_URL)

### Notice Setting
- Notice Type: Set the format of the OSS notice that can be issued.

### SMTP Setting
- Mail Server : SMTP Host (e.g. smtp.gmail.com)
- Email Address : Sender email address (e.g. no-reply@fosslight.org)
- Port : SMTP Port number (e.g. 25 or 587)
- Encoding : Default UTF-8 (Change only if necessary)
- Username : SMTP username (usually the same as the sender's email address)
- Password : SMTP user password (Password is encrypted and stored, if blank, existing password is not changed.)

### Workspace Path Setting
- Root Path : Top workspace path of upload/download file storage
