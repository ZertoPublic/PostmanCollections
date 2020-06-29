# Restore VM from LTR
Example collection to restore a selected VM from an LTR Repository

## Legal Disclaimer
This script is an example script and is not supported under any Zerto support program or service. The author and Zerto further disclaim all implied warranties including, without limitation, any implied warranties of merchantability or of fitness for a particular purpose.

In no event shall Zerto, its authors or anyone else involved in the creation, production or delivery of the scripts be liable for any damages whatsoever (including, without limitation, damages for loss of business profits, business interruption, loss of business information, or other pecuniary loss) arising out of the use of or the inability to use the sample scripts or documentation, even if the author or Zerto has been advised of the possibility of such damages. The entire risk arising out of the use or performance of the sample scripts and documentation remains with you.

## Using this Collection
**Minimum Zerto Version: 8.0 Update 2**

Import both files into your Postman environment. Doing this will create a collection called "Restore VM API (Credentials Required)" as well as an environment with declared variables that will be required during the session.

Using the environment editor, update the "address" and "port" variables as required to enable communication to the ZVM that is attached to your LTR repository. All of the other variables will be auto updated as the requests in the collection are executed.

Finally, open the "Start Session" and update the Authorization tab to provide a username and password that has appropriate access to the Zerto virtual manager. Now that the request has a username and password, send the request. Once you successfully authorize, your authorization token will be automatically created and stored in your current Environment.

From here run the commands in order as each one depends on the one before it. One thing to note is that when running the "Get VMS that exist in any backup set" and "Get Retention Sets for a VM" the test portion of the request will automatically select the first object that is returned and set this value to the auto-generated environment variable. Should you want to test with a specific VM and Retention Set, manually select and update the environment variable as desired.

Once you have completed the last request, "Post Restore VM", you should see the operation kick off in your Zerto Virtual Manager.
