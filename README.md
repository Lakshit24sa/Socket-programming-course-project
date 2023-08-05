# Socket-programming-course-project
In this assignment, I have build a simple client-server system, where you use the client to
chat with a "math" server. 
# The protocol between the client and server is as follows.
● The server is first started on a known port.
● The client program is started (server IP and port is provided on the commandline).
● The client connects to the server, and then asks the user for input. The user enters a
  simple arithmetic expression string (e.g., "1 + 2", "5 - 6", "3 * 4"). The user's input is sent to
  the server via the connected socket.
● The server reads the user's input from the client socket, evaluates the expression, and
  sends the result back to the client.
# I have written two versions of the server as instructed in the assignment :
● My server program "server1" will be a single process server that can handle only one
client at a time. If a second client tries to chat with the server while one client's session
is already in progress, the second client's socket operations should see an error.
● My server program "server2" will be a multi-process or multi-threaded server that will
fork a process for every new client it receives. Multiple clients should be able to
simultaneously chat with the server.
