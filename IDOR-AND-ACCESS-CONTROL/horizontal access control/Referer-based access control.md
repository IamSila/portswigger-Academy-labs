# lab details
- This lab controls access to certain admin functionality based on the Referer header. You can familiarize yourself with the admin panel by logging in using the credentials administrator:admin.

- To solve the lab, log in using the credentials wiener:peter and exploit the flawed access controls to promote yourself to become an administrator. 


# recon
## administrator
### upgrade user
- GET  /admin-roles?username=carlos&action=upgrade
- referer: lab_url/admin
- nothing in the request body


# SOLVING THE LAB
- make the request to /admin-roles?username=wiener&action=upgrade
notice you get unauthorised after sending that request...
- mmh i've never seen any totally secure...
- go to referer and add /admin to base url,,,
- send the request again... observe you make yourself an admin...
- congratulations, you have solved the lab..



HAPPY HACKING :)
