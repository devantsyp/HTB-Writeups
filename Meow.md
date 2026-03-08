# HTB Lab - Meow - Very Easy - Linux - 3/8/2026  

## Key Takeaways
- OpenVPN is the service HTB uses to establish a VPN connection to Labs.  
- PING is a tool (terminal command) used to test connection to a target using ICMP echo requests.  
- NMAP (Network Mapper) is a tool for network discovery and finding open ports on target.
 - Telnet is an older, text-based network protocol and application typically running on port 23.  
- Telnet allows the user to connect to and interact with a remote computer's CMD line via TCP/IP. Largely replaced by SSH due to lack of encryption.

## Commands used
- **nmap -sC 10.129.7.90**  
  Used to scan for open ports at target 10.129.7.90.
  Identified port **23/tcp** in **Open** state running on **telnet** service.
  
- **telnet -l root 10.129.7.90**  
  Used to log into a remote system as user **root** specified with **-l** flag using the Telnet protocol.

- **whoami**  
  Used to return the current logged in user.
