<h1>The completed evidence table with three distinct public IPv4 addresses:</h1>

<table>
  <thead>
    <tr>
      <th>Deployment</th>
      <th>Public IPv4 address</th>
      <th>Connection method</th>
      <th>Screenshot</th>
      <th>Instance terminated?</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>18.118.216.93</td>
      <td>SSH</td>
      <td>deployment-1.png</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td>2</td>
      <td>3.143.110.232</td>
      <td>SSH</td>
      <td>deployment-2.png</td>
      <td>Yes</td>
    </tr>
    <tr>
      <td>3</td>
      <td>3.132.212.97</td>
      <td>SSH</td>
      <td>deployment-3.png</td>
      <td>Yes</td>
    </tr>
  </tbody>
</table>
#
<h1>Deployment description:</h1> (launch, SSH connection, and dashboard) 

<h3>Deployment #1 :</h3>

<h3>Deployment #2 :</h3>

<h3>Deployment #3 :</h3>

<h1>Instance Data Refleciton:</h1>

<h3>Host Name:</h3> ip-172-31-28-74.us-east-2b.compute.internal

<h3>Instance type:</h3> T3. Micro 
Reflection:
the Virtual Machine size

<h3>Availability Zone:</h3> us-east-2b
Reflection: 
The Virtual Machine (ec2) is physically hosted inside the region

<h3>CPU:</h3> 0% busy (approx.) | 2 vCPU(s)
Reflection: ip-172-31-28-74.us-east-2b.compute.internal
The server is idle
Not under heavy load

<h3>Memory:</h3>  180Mi used / 913Mi total
Reflection:
Roughly 20% used
Plenty of memory available

<h3>Disk:</h3> 1.7G used / 8.0G total (21% full)
Reflection:
Only 21% full
About 6.3 GB free
Nothing alarming

<h3>Uptime:</h3> up 9 minutes
Reflection:
Instance running for a short time

<h1>The one thing that became easier after repeating the process:</h>

Creating instances began more natural after creating 3 and working through some kinks


<h>Errors encountered and resolution:</h>

#1. Upon accessing my ec2 instance I used the command line # ssh -i ec2-user@"my_public_IPv4" and was rejected from connecting to my AWS EC2 instance. I then investigated and confirmed my Instance Passkey was required and implemented the key in to the command line # ssh -i "Passkey" ec2-user@"my_public_IPv4". After submission I then was prompted whether I wanted to proceed. Once I acknowledged "yes" I then obtained authorization to connect to the ec2 server.  

#2. After obtaining authorization to access Sear Foundation output did not display. I realized that I did not appliy the Raw Code from the repository when creating my ec2 instance. I terminated the ec2 and started fresh. Acquired the ec2 Raw code from the reposity and applied it to my new ec2 instance.

#3. In addition I terminated my old security and created a fresh one. My inbound rules were set for "SSH" and " "HTTP" and instead of using IP4V as the source I selected "My IP" to not open the "SSH" and "HTTP" to the entire internet.


<h>Practice instances clean up:</h1>

Instances Terminated