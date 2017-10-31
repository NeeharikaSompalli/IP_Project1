# IP_Project1
  Makefile
Unity Id:nsompal, nvenugo2

This Project Runs on Ubuntu and is coded ins Java.

1. Compile and run RSServer.java from IP_Project_Code/src folder by the following command
                                   javac RSServer.java
    Run “ java RSServer” to run the Server.


2. Compile and run PeerClient.java IP_Project_Code/src folder by the following command
                                  javac PeerClient.java
   Run  “java PeerClient” to run Peer.

3.  The PeerClient  asks for the following inputs:

Enter the RFC file path
<give the file path  of all rfcs for that peer> 
( It resides on  IP_Project_Code/src/rfcfile1 to  IP_Project_Code/src/rfcfile6)
All 60 RFCs are present in IP_Project_Code/src/rfcfile1

Enter the  (Peer) Host port number
<Give the port number on which this peer runs> eg:65422

Enter the  Peer IP address
<Give the IP address of the machine on which Peer runs> eg:10.139.63.91

Enter the  RS Server IP Address
<Give the IP address of the machine on which RSServer program runs>       eg:10.139.60.50
      
  Enter your choice number
 
 1. Register 
 2. Leave 
 3. Keep Alive 
 4. PQuery  
 5. RFCQuery 
 6. GET RFC 
 7. Task 1 and Task 2 Output 
 8. Terminate

Run the Commands in the following order to download one specific RFC.

1. Register the Peer with RS Server(option1)
2. Run PQuery(option 4) to get the list of all active peers in the system.
3. Run RFC query(option 5) to get the list of all RFCs present in the system with other peers
4. Give GET RFC(option 6) and it prompts asking which RFC file needs to be downloaded. Give the file needed in the format <rfcfilenumber>.pdf (Eg:1234.pdf) . This will download the specific RFC to the file path. 
5. For any peer to leave the system give Option 2 and the TTL value is reset to 0 and the active status flag is set to false.
6. If the peer wants to reset TTL value to 7200 after the TTL value goes to 0 , give option 3 Keep Alive.

Please make sure to run Steps in the following order for Task1 and Task2 Outputs:

 Task1:

Make sure to have 60 RFC files in one folder.( IP_Project_Code/src/rfcfile1)

1. Register all 6 peers with RS Server(Give option 1)
2. Run PQuery (Option4)on all 6 peers. It returns all the active peers in the system.
3. Run RFC Query(Option 5) on all 6 peers. It gives the list of all RFCs present in all other peers in the system.
4. Run Option 7 and give 2 for Task 1 and Enter number of RFCs required to be downloaded as 50. This will download all the 50 RFCs to the folder specified.
5. This will display the cumulative file download time when each file is downloaded on the console.


 Task2:

Make sure to have 10 RFC files in each folder.( IP_Project_Code/src/rfcfile1 to IP_Project_Code/src/rfcfile6)

1. Register all 6 peers with RS Server(Give option 1)
2. Run PQuery on all 6 peers. It returns all the active peers in the system.
3. Run RFC Query on all 6 peers. It gives the list of all RFCs present in all other peers in the system.
4. Run Option 7 and give 1 for Task 2 . This will contact all other Peers with the specified RFCs and download all other RFCs other than RFCs it has.
5. This will show the cumulative time taken  to download when each file is downloaded in the console.


