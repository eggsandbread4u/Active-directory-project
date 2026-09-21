# Active-directory-project
Learn how to set up users and groups and manage them

# Set up a domain controller (DC) and a client PC
The first step is to set up the environment. A window sever 2025 for domain controller as it comes with a server manager and for a client PC window 11 enterprise. A domain controller manages all the login, password checks, authorization, and authentication
<img width="1886" height="852" alt="Screenshot 2026-09-21 095753" src="https://github.com/user-attachments/assets/920fd03a-41a3-4004-b155-9d96a0808cb7" />
Once that's done you'll install active directory tools by clicking on manage tab and select 'Add roles and features' From server role you can download a variety of roles.
<img width="894" height="580" alt="Screenshot 2026-09-21 100219" src="https://github.com/user-attachments/assets/3e8b1e85-70b1-41c6-bbfb-a1a82344352d" />
To see whether the desired roles have been installed you can simply click on the tools tab and check 
<img width="342" height="233" alt="Screenshot 2026-09-21 100359" src="https://github.com/user-attachments/assets/6c9307a0-311c-4e55-88d4-1d37ffb94c9d" />

# Setting up your first user
To set up a user go to tools tab and click on 'Active directory Users and Computers'
<img width="622" height="186" alt="Screenshot 2026-09-20 191713" src="https://github.com/user-attachments/assets/dc14618b-aea3-4c05-9c8e-166087b9175d" /> 
You'll see a bunch of folders click on your domain and make a OU folder. Inside that OU folder make sub-OU folders 'IT' and 'sales' 
<img width="192" height="57" alt="Screenshot 2026-09-20 191827" src="https://github.com/user-attachments/assets/9052be1b-c36e-4442-b648-959867848cb1" />
<img width="439" height="331" alt="Screenshot 2026-09-20 191757" src="https://github.com/user-attachments/assets/5399f65f-b1bb-4723-9cb0-46b85524f924" />
Now right click one of the folders and make a user inside them. A window will pop up that will ask you to set up the user name and password and also the user ID
<img width="450" height="388" alt="Screenshot 2026-09-20 191954" src="https://github.com/user-attachments/assets/fd9b76db-0ce5-4167-afb7-7c6777de1c8f" />
Once you've created a user you can click on it and make new changes if you wish to
<img width="554" height="599" alt="Screenshot 2026-09-20 192013" src="https://github.com/user-attachments/assets/39011ea4-cb24-4b04-9539-5e56517c9c62" />

# Logging in as the new user
On your client PC, go to the log in screen and click other user. You'll be asked to enter the username and the password. Enter the new user's username along with the password. Remember the user name must look like this 'user@[your domain name].local'
<img width="866" height="533" alt="Screenshot 2026-09-20 192045" src="https://github.com/user-attachments/assets/e00d98e0-af17-4732-af02-83fe2b9c416d" />
You'll be logged in as new user with the permissions and privileges according to your category and domain. To make sure you're logged in as your new user's profile simply write whoami on command prompt to be sure
<img width="850" height="339" alt="Screenshot 2026-09-20 192458" src="https://github.com/user-attachments/assets/1dd703e2-41da-47b7-9d4e-c1a2f8957b19" />










