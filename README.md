# Coding-Royale
## Game explanation
A battle royale game in which the objective is to finish a series of short chalanges. Each challenge is to debug a small program, when a challenge is completed, all other players recieve a pentalty (a series of forced keystrokes). The goal is to finish all challenges before any other players. The more players the more fun!

## Client
Just download and run the .exe file in the root directory and fill out the blanks (IP is that of server). **Note: Useless without a server, delete java files manually.**
## Server
The server contains all necesary files except an FTP server, just run server.ahk (you need autohotkey) and an FTP server (I use filezilla). The FTP server should be set up to where each user has their "home" directory in _/Clients/**name**/_, but if you use filezilla, you can use the built-in reset and server location features to update the server's user list automatically. Be sure to not add a trailing slash to the path of the server location (ex: _C:/Users/Simonomi/Desktop/FileZilla Server_, not  _C:/Users/Simonomi/Desktop/FileZilla Server/_). If the reset feature isn't updating the server's users, try pressing it again and checking that the path is correct.
Players.ini (editable through server.ahk) should look similar to the following:<br/>

_TotalPlayers=2<br/>
Player1=FirstPlayer<br/>
Player2=SecondPlayer_
## Challenge packs
There is now a challenge pack creator that can be used to easily create challenge packs. Select two files for each challenge: a .orig for the unsolved version, and a .java for the solved version. To change the randomly generated order, edit the challenges.ini file.
### Note: Built for Windows 10

## Possible future changes
1. Change challenges to use "solved" version instead of **name**goal.txt
2. Make seperate challenge pack creator (xor with #1)
3. Client.exe delete java files (from game only)
