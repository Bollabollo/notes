# Hosts File
In the early days of computer networking, people just write down the IP addresses of computers they need to connect to on their desk. 

The hosts file was the 1st attempt to create a centrally managed table of computer names and addresses, distributable by the network administrator. The hosts file is local and is often different on each machine.

It's used before the birth of the DNS to perform a name to IP address matching. It's a simple text file but **doesn't have .txt extension.**

### When it is used
It maybe used depending on the local computer name resolution configuration (dk what that is - **look up later**) and is used before all other methods. **RELATED TO PING COMMAND FOR CLI:** When you ping a website, the ping command will resolve the name to an ip address (DNS). So if I understand this correctly, the hosts file resolve the name of the website on the right column to the IP address on the left column. So when I routed my banned websites to 0.0.0.0 (invalid, non-existent ip address), I am resolving the name of these websites I enter into my web browser to this 0.0.0.0 IP address --> which resolves in error.

**USE THIS FOR MAKING WEBSITE**
