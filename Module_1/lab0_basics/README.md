The completed evidence table with three distinct public IPv4 addresses:
Deployment	Public IPv4 address	Connection method	Screenshot	        Instance terminated?
1	        18.118.216.93	         SSH	        deployment-1.png	Yes
2	        3.143.110.232	         SSH	        deployment-2.png	Yes
3	        3.132.212.97	         SSH	        deployment-3.png	Yes

Deployment description: (launch, SSH connection, and dashboard) 


Deployment #1 :

Deployment #2 :

Deployment #3 :

Instance Data Refleciton:

Instance type / Availability Zone: T3. Micro

CPU: 0% busy (approx.) | 2 vCPU(s)
Reflection:

The server is idle
Not under heavy load

Memory:  180Mi used / 913Mi total

Reflection:
Roughly 20% used
Plenty of memory available

Disk: 1.7G used / 8.0G total (21% full)

Reflection:

Only 21% full
About 6.3 GB free
Nothing alarming

Uptime: up 9 minutes

Reflection:
Instance running for a short time

The one thing that became easier after repeating the process:

Creating instances began more natural after creating 3 and working through some kinks


Errors encountered and resolution:

1. Upon accessing my ec2 instance I used the command line # ssh -i ec2-user@"my_public_IPv4" and was rejected from connecting to my AWS EC2 instance. I then investigated and confirmed my Instance Passkey was required and implemented the key in to the command line # ssh -i "Passkey" ec2-user@"my_public_IPv4". After submission I then was prompted whether I wanted to proceed. Once I acknowledged "yes" I then obtained authorization to connect to the ec2 server.  

2. After obtaining authorization to access Sear Foundation output did not display. I realized that I did not appliy the Raw Code from the repository when creating my ec2 instance. I terminated the ec2 and started fresh. Acquired the ec2 Raw code from the reposity and applied it to my new ec2 instance.

3. In addition I terminated my old security and created a fresh one. My inbound rules were set for "SSH" and " "HTTP" and instead of using IP4V as the source I selected "My IP" to not open the "SSH" and "HTTP" to the entire internet.


Practice instances cleaned up:

Instances Terminated