<h1> The completed evidence table with three distinct public IPv4 addresses:</h1>

| Deployment | Public IPv4 address | Connection method | Screenshot | Instance terminated? |
|-----------|---------------------|-------------------|-----------|----------------------|
| 1 | 18.118.216.93 | SSH | deployment-1.png | Yes |
| 2 | 3.143.110.232 | SSH | deployment-2.png | Yes |
| 3 | 3.132.212.97 | SSH | deployment-3.png | Yes |

<h1>Deployment description:</h1> (launch, SSH connection, and dashboard) 

<h2>Deployment #1 :</h2>
![Deployment 1](screenshots/deployment-1.png)

<h2>Deployment #2 :</h2>
![Deployment 2](screenshots/deployment-2.png)

<h2>Deployment #3 :</h2>
![Deployment 3](screenshots/deployment-3.png)

<h1>Instance Data Refleciton Deployment #1:</h1>

<h3>Host Name:</h3> ip-172-31-28-74.us-east-2b.compute.internal

<h3>Instance type:</h3> T3. Micro 
Reflection:
the Virtual Machine size

<h3>Availability Zone:</h3> us-east-2b
Reflection: 
The Virtual Machine (ec2) is physically hosted inside this region

<h3>CPU:</h3> 0% busy (approx.) | 2 vCPU(s)
Reflection: ip-172-31-28-74.us-east-2b.compute.internal
The server is idle
Not under heavy load

<h3>Memory:</h3>  180Mi used / 913Mi total
Reflection:
Roughly 20% of Mebibytes used
Plenty of memory available

<h3>Disk:</h3> 1.7G used / 8.0G total (21% full)
Reflection:
Only 21% Gigabytes occupied
About 6.3 GB free
Good on threshold

<h3>Uptime:</h3> up 9 minutes
Reflection:
Instance running for a short time

<h1>The one thing that became easier after repeating the process:</h>

Creating instances began more natural after creating 3 and working through some kinks

<h1>Errors encountered and resolution:</h1>

#1 Upon accessing my ec2 instance I used the command line # ssh -i ec2-user@"my_public_IPv4" and was rejected from connecting to my AWS EC2 instance. I then investigated and confirmed my Instance Passkey was required and implemented the key in to the command line # ssh -i "Passkey" ec2-user@"my_public_IPv4". After submission I then was prompted whether I wanted to proceed. Once I acknowledged "yes" I then obtained authorization to connect to the ec2 server.  

#2 After obtaining authorization to access Sear Foundation output did not display. I realized that I did not appliy the Raw Code from the repository when creating my ec2 instance. I terminated the ec2 and started fresh. Acquired the ec2 Raw code from the reposity and applied it to my new ec2 instance.

#3 In addition I terminated my old security and created a fresh one. My inbound rules were set for "SSH" and " "HTTP" and instead of using IP4V as the source I selected "My IP" to not open the "SSH" and "HTTP" to the entire internet.


<h1>Practice instances clean up:</h1>

Instances Terminated

<h1>Assignment Completion Checklist</h1>

- [x] I connected to AWS EC2 using SSH.
- [x] I observed the SEIR dashboard raw code.
- [x] I completed three separate EC2 deployments for homework.
- [x] I successfully connected to each of the three instances.
- [x] I recorded three distinct public IPv4 addresses.
- [x] I uploaded three SEIR dashboard screenshots and explanations to my GitHub repository.
- [x] I submitted my repository link by Tuesday, October 20, 2026, noon Central Time.
- [x] I terminated unused EC2 instances and checked for leftover billable resources.