# Update Service Account Credentials
Example collection to update the username and password of the service account used by the Zerto Virtual Manager to connect to the hypervisor environment.

## Legal Disclaimer
This script is an example script and is not supported under any Zerto support program or service. The author and Zerto further disclaim all implied warranties including, without limitation, any implied warranties of merchantability or of fitness for a particular purpose.

In no event shall Zerto, its authors or anyone else involved in the creation, production or delivery of the scripts be liable for any damages whatsoever (including, without limitation, damages for loss of business profits, business interruption, loss of business information, or other pecuniary loss) arising out of the use of or the inability to use the sample scripts or documentation, even if the author or Zerto has been advised of the possibility of such damages. The entire risk arising out of the use or performance of the sample scripts and documentation remains with you.

## Using this Collection
**Minimum Zerto Version: 8.0 Update 2**

Import both files into your Postman environment. Doing this will create a collection called "Update Service Account Credentials" as well as an environment with declared variables that will be required during the session.

Using the environment editor, update the "address" and "port" variables as required to enable communication to the ZVM as well as the "New_Username" and "New_Password" variables. Note, both items are required, even if the username is going to remain the same.

Finally, open the "Start Session" and update the Authorization tab to provide a username and password that has appropriate access to the Zerto virtual manager. Now that the request has a username and password, send the request. Once you successfully authorize, your authorization token will be automatically created and stored in your current Environment.

Now that you have successfully authenticated to the Zerto Virtual Manager, run the next function "Update Service Account Credentials." This will update the UserName and Password to the new values.
