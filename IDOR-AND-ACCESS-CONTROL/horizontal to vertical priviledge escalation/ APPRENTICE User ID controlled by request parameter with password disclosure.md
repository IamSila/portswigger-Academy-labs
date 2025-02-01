# lab details
-  This lab has user account page that contains the current user's existing password, prefilled in a masked input.

- To solve the lab, retrieve the administrator's password, then use it to delete the user carlos. 


# recon
- attacker account -> wiener:peter

## my-account page
- /my-account?id=wiener


# solution
change the user to id from wiener to carlos, realise you can access another user's account.... the password input is also prefilled with the user's password...intresting..

now using carlos:and the password,  you access carlos account...

try changing id to admin and it redirect to login...

try changing id to administrator and you access admin account, retrieve the pass and log in as admin...

delete carlos account to solve the lab...


HAPPY HACKING :)

