# LevelUpBot
A Steam NodeJS bot that trades full sets of trading cards for keys.

How to get your shared_secret & identity_secret:
<br>1: Go to the SDA(Steam Desktop Authenticator) directory. If you have encryption disabled go to step 3.
<br>2: Open SDA and hit "Manage Encryption". Fill in your encryption key and when asked to create a new one leave the text box blank. This will disable encryption.
<br>3: Head over to the maFiles folder and open the file named after your accounts SteamID64.
<br>4: Search the file for shared_secret:"XXXXXXXXXXXXXX=", instead of XXX it should have a code there, it always ends with =
<br>5: Do the same for identity_secret, it will look similar.
<br>
<br>How to set up a server with DigitalOcean
<br>1: Add funds, and create a Droplet. Hit "One Click Apps" and select NodeJS.
<br>2: Once created, download Putty and Filezilla: https://filezilla-project.org/ & http://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html
<br>3: Open Putty, fill in the IP address sent to your e-mail and wait for the command prompt to open. Once opened fill in username "root" and the password sent to your email. You can copy your password in your email and paste it in Putty using right click, you wont see your password!
<br>4: It will ask you to fill in the password again, fill it in and fill in a new password and confirm it.
<br>5: Once you're done run the command: npm install -g forever. This allows the server to run the bot without a Putty window being opened.
<br>6: Now open FileZilla and connect to your server, username = root and the password is the password you've just set, port = 22.
<br>7: Drag the bot files in, wait for this to complete and head back to Putty.
<br>8: Run the command: npm i
<br>9: To start your bot run this command in Putty: forever start index.js
<br>Then your bot should be running!
<br>Make sure to fill in the config!

<br><br><br>Errors, issues, bugs or problems? https://github.com/lejzylimz/LevelUpBot/issues !

