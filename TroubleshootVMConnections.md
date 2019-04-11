# Troubleshooting 
### Errors Interacting with Ushahidi within VM
1. Following Step 10 in Ushahidi VM Installation.md, open a MATE Terminal in the VM.
1. Change the directory to platform-client ("cd platform-client")
1. View directory contents ("ls -a") and ensure there is a .env file
1. Use 'cat .env' to view contents of .env
1. Run "ifconfig" to ensure Enpos8's inet address matches the address located in step 13b (Second Wired Connection listed)
1. If the addresses __do not match__:
    * Run 'pluma .env' to open a simple text editor
    * Edit and save the BACKEND_URL so that it matches the address of the connection found in step 13b
1. Run 'cat .env in terminal again to ensure it was correct.
1. Run 'npm run watch' 
    * Two URLs should be present
    * To use the local URL - click it

__Note:__ You should be consistent with step 12 now 
