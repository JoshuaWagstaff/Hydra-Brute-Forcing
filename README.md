# Writeup
# Hydra Brute Forcing

## Objective
Brute-force the web login and then the SSH account for user molly on the Hydra Challenge box to retrieve both flags.

### Skills Learned

Intercepting and inspecting a POST-login request in Burp Suite to identify the failure message.

-Crafting a Hydra http-post-form command, including the correct field names and “failure” string, to crack the web password.

-Reading Hydra’s verbose output to identify successful credentials.

-Switching to the SSH module in Hydra to perform a second brute-force attack.

-Extracting the discovered SSH password from Hydra’s result

### Tools Used

-Hydra (thc-hydra) for both HTTP-form and SSH brute-forcing

-Burp Suite Community Edition for capturing/intercepting the login POST

-rockyou.txt wordlist (located at /usr/share/wordlists/rockyou.txt)

-Standard SSH client to log in once credentials were recovered

## Steps
---
Ref.1: Password we're brute forcing
<img width="546" alt="1- password we're brute forcing" src="https://github.com/user-attachments/assets/17a69b10-bef0-424d-b4ad-345c6c3a9f18" />
---
Ref.2: Make sure intercept is on in burpsuite
<img width="777" alt="2 - make sure intercept is on in burpsuite" src="https://github.com/user-attachments/assets/1763a038-1504-4ab5-9f1c-71eb298b922e" />
---
Ref.3: Try random password to intercept in burpsuite
<img width="785" alt="3- try random password to intercept in burpsuite" src="https://github.com/user-attachments/assets/a10d2a88-ff0c-4705-b441-ee2fae82d0f7" />
---
Ref.4: save this phrase to input in terminal
<img width="314" alt="4- save this phrase to input in terminal" src="https://github.com/user-attachments/assets/469ab5c8-c3ce-4880-8c40-e807263c28ef" />
---
Ref.5: Hydra brute force command
<img width="593" alt="5- hydra brute force command" src="https://github.com/user-attachments/assets/191e9924-45ad-4081-b45a-b3852b86c3d4" />
---
Ref.6: Found the user and pass through brute forcing
<img width="560" alt="6- found the user and pass through brute forcing" src="https://github.com/user-attachments/assets/e67ee4c7-bdce-4aea-806a-1d9f456564d3" />
---
Ref.7: Broke In
<img width="1262" alt="7 -broke in" src="https://github.com/user-attachments/assets/c08a8ea7-80c3-4e74-a60f-5c741758c070" />
---
Ref.8: Now must brute force SSH password
<img width="529" alt="8- now must brute force ssh password" src="https://github.com/user-attachments/assets/307ebebf-fa07-4bf5-8c86-a3e93a09957c" />
---
Ref.9: SSH command
<img width="569" alt="9- ssh command" src="https://github.com/user-attachments/assets/e64ebfaf-fd1f-4003-92a7-0ba456e611bd" />
---
Ref.10: Password cracked
<img width="534" alt="10- password cracked" src="https://github.com/user-attachments/assets/1e8ea051-898f-46cc-9431-f641ec7912e1" />
---
Ref.11: Successful login
<img width="440" alt="11- succesful login" src="https://github.com/user-attachments/assets/1834a705-cda9-44c5-b4ca-0a62a0b864be" />
---































