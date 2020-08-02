The project has been referenced from
https://www.dreamincode.net/forums/topic/259777-a-simple-chat-program-with-clientserver-gui-
optional/
https://www.techiedelight.com/periodically-execute-task-java//
https://stackoverflow.com/questions/44087399/using-javas-executor-service-with-a-non-static-m
ethod
Steps to run the project:
1) Import the project named ChatApp.
2) Run ServerGUI.java for starting the server.
3) Run ClientGUI.java for the client’s GUI.
Here for logging in with a user, we need to give a unique username to the GUI of the client and
then click on the Login button.
If there are 3 clients then every client will randomly pick a client to send its respective vector
clock every 8 seconds.
For logging-out, we need to click on the Logout button.
For checking the clients’ list which is already connected to the server we need to press the
“Existing users” button and when we will start the server, then also active clients’’ list will be
displayed in a dialog box.
The “Existing users” button will be disabled when the user is not logged in but the server will
know which are connected clients.
After every 8 seconds, any client will send its clock to any other client but only when the number
of connected clients is 3.
We need to run ClientGUI.java multiple times in order to add different clients to the server.
If we try to connect a new client who has the same username as any existing user, then it will
show a pop-up message that “Username already exists”.
The server can have only up to 3 clients connected to it at a single time. And if we try to connect
the server to the 4th client then it will show a pop-up message that “Cannot connect more than 3
users”.Server GUI will contain a log of each connected user and the clocks that the sent with the
corresponding recipients.
