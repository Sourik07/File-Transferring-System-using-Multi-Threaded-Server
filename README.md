# Multithreaded-File-Server
![pc-to-pc](https://github.com/Sourik07/Multithreaded-File-Server/assets/113095592/d4bb1c6d-b661-497c-a3c7-c60d82b15767)

The File Transferring System using the Multi-Threaded Server project is a software application that enables the efficient and reliable transfer of files between multiple clients and a central server. The system is designed using a multi-threaded server architecture to handle multiple clients concurrently, improving the overall system performance.

i)	Domain Description
Our MFS can allow a maximum of 4 multiple clients to upload as well as download from the server concurrently. This maximum number can be increased as per need and it will require much more powerful hardware.
MFS uses the Thread Pool to handle threads MFS.


ii)	Motivation
Let’s take an example, say there is an office consisting of 100 employees and these employees are working in different departments and they need to share files with each other. With MFS, employees can just upload their files to the Server and other employees can easily download it into their respective PC


iii)	Scope
The features available to the Clients are:
• Can upload a file of max size approx 260 bytes. But it depends on the storage size available on the server. If the storage size in the server is 5TB then clients must to not upload file size more than 5TB
• Can make a request to upload multiple files at the same time. 
• Can download any number of files at the same time.
• The client can set permissions for each uploaded file

Screenshot

Uploading a File
![Picture1](https://github.com/Sourik07/Multithreaded-File-Server/assets/113095592/9ae8c726-a652-4ec1-ab53-b2b499ef0aac)

Downloading a File
![Picture2](https://github.com/Sourik07/Multithreaded-File-Server/assets/113095592/24d91bfc-0144-4959-8115-ce49a07ccd6b)

Running the Server:
javac -cp '.:jar_files/server/*' ClientHandler.java;
javac -cp '.:jar_files/server/*' ServerDriver.java && java -cp '.:jar_files/server/*' ServerDriver
