# User ID controlled by request parameter 
goal - retrieve another user's api key and submit

target user : carlos


## recon
### my account details
- wiener:peter
- Your API Keyis:wRCHylfG2sNrHtBq8mcacGFRZYPGNI63
    #### navigating to account details
    - Observe how the email is like for retrieving the account details for wiener *https://0a3c00c6030fd868826ebf8900ca00d4.web-security-academy.net/my-account?id=wiener*
    - Notice that id=carlos

solving:
- change the id parameter to carlos like such:
https://0a3c00c6030fd868826ebf8900ca00d4.web-security-academy.net/my-account?id=carlos

- Observe you have carlos details while logged in as wiener

- Always check how the app fetches user's details... 

- Try to modify these parameters and point to another user you own such as your second account...


HAPPY HACKING :)