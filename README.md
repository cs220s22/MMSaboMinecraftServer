# MMSaboMinecraftServer

To Run On Local Docker Container:
===
1. make sure docker desktop is running
2. type " docker-compose up " in command line to build and run the server on docker
3. cd mcrcon-0.72
4. compile RCON cc -std=gnu99 -Wpedantic -Wall -Wextra -Os -o mcrcon mcrcon.c
5. to connect rcon to server run  ./mcrcon-0.7.2/mcrcon -H localhost -p password123 -P 25575

To Run Locally:
===
1. run command in .server-data/  :   java -Xmx4G -jar paper-1.17.1-408.jar nogui


To Run On AWS EC2 Instance:
===
1. Create a t2.large ec2 instance using the Amazon Linux 2 AMI and 64-bit (x86) architecture
2. specify a key login pair
3. create a security group with the following rules:
    * Inbound: SSH on port 22 with with the source being anywhere IPv4
    * Inbound: TCP Custon on port 25565 with with the source being anywhere IPv4
    * Outbound: All traffic on all port ranges
4. Run the instance
5. run script?


!!! make script for local
figure out environment variable


