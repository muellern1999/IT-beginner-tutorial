# IT-beginner-tutorial By Nathan Mueller
A place for people with little to no IT experience. 
We shall be going over basic hardware troubleshooting techniques for cisco switches and routers

Step 1 the very first thing you want to do is always check the physical connections. (does it have power is it plugged into the wall?)
this includes anything it should be connected to via a cable make sure they are all plugged in and the cable has no obvious damage.

Step 2 login with your username and password

Step 3 enter priveledged mode (assuming you have admin status in the machine) by typing enable and entering another password

Step 4 one of the easiest ways to check for any problem throughout a switch or router is to use the command "show run"

Step 5 show run will show you the running config of the current machine and as such it is a convienent place to look for what could be wrong here are just a few things that easily go wrong that you can find in a show run (ip addresses, routes, vlans, password encryption, what ports are open/closed, etc)

Step 5 identify your problem now this is kind of tricky. There are many things that can gowrong with a switch or router and they are to many to cover in one tutorial so for now I will not be solving your specific issue.

Step 6 after you have identified the issue in your machine you have to go to the proper config type to edit it (eg you have to be in switchport mode to edit ports on a switch)

Step 7 make the neccessary changes, for instance type the command "service password-encryption" to encrypt the passwords on your device

Step 8 move back down from your current config mode to global config and type "show run" again (if the command doesn't work you aren't in the correct config mode although you can get around it by using the command "do show run")

Step 9 scan for the change you made and if it is in there check to make sure it works correctly

Step 10 if the change you made works correctly type the command "copy run start" or alternatively "write mem" to save the running config (what you just changed) to the start config (what the device will boot up to if reset)
