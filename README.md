# scripts
In this repository are a group of scripts that I used to create an ElkStack for my cybersecurity class, along with a diagram of how the system is set up.
If you wish to set one up, the first step is to create a security group with the relevant security rules.
When setting up security rules, you should ideally only allow traffic on the ports you wish to use, and from known/trusted IP addresses (this may have to be updated over time).
Then create a jump box. From the jumpbox, utilize ansible/docker and the scripts provided to set up your containers. 
You will have to update the hosts file from the jump box with the ansible containers, along with updating your security rules to allow the ports/IP addresses that you use. 
Once that is set up, run docker and you should be able to enter the containers themselves. 
Once that is completed, you can set up metricbeat and filebeat, using the files provided in this repository, to track/organize relevant logs for your system.
Good luck!
