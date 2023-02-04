# Lab 2
[Fork](https://docs.github.com/en/get-started/quickstart/fork-a-repo) this repo and clone it to your machine to get started!

## Team Members
- team member 1
- team member 2

## Lab Question Answers

Answer for Question 1: 
The reliability of transmission decreased when we set a 50% loss to our local environment. The 'netem' command provides network emulation functionality enables us to specify what percentage of packets are reordered. Packets that have been reordered results in data loss.

Answer for Question 2:
TCP maintains its reliability because TCP would make sure that the client always receives the packet. If the packets are lost, TCP would make the server resend them until they are received by the client.

Answer for Question 3:
The speed of the response time decreases because the server constantly drops 50 percent of its sent packets. The server has to resend again and again which makes the response time longer. Also, the fact that TCP requires client to present data in order makes the response time longer . The arrived packets have to wait to be presented until all of their prior ones are received.

C++
 
Question 1: 
ARGC represents the number of arguments passed to the program through the command line interface. ARGV is an array of pointers that contains said arguments passed to the program. 

Question 2:
A file descriptor is a positive integer used by the system to represent a file, socket, pipe, or any other IO resource. 
The file descriptor table, a data structure maintained by the OS's kernel, maps file descriptors to corresponding memory addresses. Each process has its own corresponding file descriptor table. 

Question 3:
Struct is a variable type which combines different types as the user’s choices. The members of sockaddr_in are sin_family, sin_port, in_add, and sin_zero. Sin Family is a short which specifies the types of address family like iPv4 and iPv6.  sin_port is an unsigned short which tell the port number that the server uses. in_add is a structure which has a member of uint32_t telling the IP address. 
sin_zero is an array of 8 character which is used to conpensatethe size of the structure 

Question 4: 
The socket() function has a prototype of: int socket(int domain, int type, int protocol). Domain specifies the communications domain in which a socket is to be created. Type represents the type of socket to be created. Finally, protocol represents the exact protocol to be used with said socket. 
socket returns an int, whihc is a file descriptor for a new socket. The function can also return a -1 along with the error number should something go ary.

Question 5:
The bind function's prototype is as follows: int bind(int sockfd, const struct sockaddr *addr, socklen_t addrlen). bind() will map a specified addr to the socket referred to by the file descriptor, sockfd. addrlen specifies the size, in bytes, of the address strcutur. bind() returns an int, which can either be a 0, which signifies sucess, or a -1 along with the error number when an error occurs.
The listen function's prototype is: int listen(intsockfd, int backlog). listen() will mark the sockfd socket as a socket which will be used to accept incoming connection requests. 


