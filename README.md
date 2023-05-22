# SimpleServerScenario

Tasks for programming classes at PJATK

A simple, example server scenario in C.

The server makes a file available and the user can download it to themselves.


The communication protocol looks like this:

CLIENT SERVER

length_file_name >

file_name[length_file_name] >

                                  < file_size

                                  < package_1[file_size].

--close connection-- --close connection--.


The server runs in a loop until CTRL+C is called, then it closes.
As a simplification, the server has no security

