# Outline
## Follow this guide and we can win
### [Taskade.com Checklist (USE ME)](https://www.taskade.com/e/zenZT5XpYQfzaGL4)
1. Map the Network
2. Record the Information
3. Change the Passwords
4. Review the Logs
5. Discover the Services
6. Remove the Unnecessary
   1. Accounts
   2. Suspicious Services
7. Close the Ports
   1. NMAP
8. Configure the Firewall
9.  Harden the Services
10. Begin the Monitoring
    
### Materials
1. [Tracker](https://www.taskade.com/v/zohsq78BuLox6HHY)
1. [Network Diagram](https://drive.google.com/file/d/1sEEQJ_LAxgnvEPPrEnLjEfR9WEuxXT2m/view?usp=sharing)
2. [Master Tracker](https://docs.google.com/spreadsheets/d/1HBHPwd_kgSvzu1PwQwOEbf7rUsc6q2Bj2oVbtZFw4EQ/edit?usp=sharing)

### Resources

# Warnings
- [ ] **DO NOT REBOOT** or shut down without clearance from the Team Leader.
- [ ] **SAVE OLD CONFIGURATION FILES** before modifying a copy.
  - [ ] `sudo su`
  - [ ] `cat /etc/test/test.conf > /etc/test/test.bac`
  - [ ] `exit`

# Map the network
`ipconfig`/`ifconfig`/`ip addr`

[Template](https://drive.google.com/file/d/1sEEQJ_LAxgnvEPPrEnLjEfR9WEuxXT2m/view?usp=sharing)
# Record machine information
# Change all passwords
[Why Diceware?](https://theintercept.com/2015/03/26/passphrases-can-memorize-attackers-cant-guess/)
# Review the logs
# Discover running services
# Remove Unnecessary things
# Accounts
# Suspicious Services
# Close the ports
# Configure the firewall
# Harden services
# Begin Monitoring

## System Reconnaissance
- [ ] Discover and record operating system and version.
	- [ ] Switch personnel onto preferred systems if possible.
- [ ] *If no credentials given*, break in.
- [ ] Log in and **change the user password**. Record the new password.  
	*USERNAME: ________________&nbsp;&nbsp;&nbsp;&nbsp;PASSWORD: ________________*
- [ ] *If no root access*, escalate privileges.
- [ ] Gain administrative access and **change the password.** Record the new password.  
	*USERNAME: ________________&nbsp;&nbsp;&nbsp;&nbsp;PASSWORD: ________________*
- [ ] Open and begin monitoring important system and service logs.
- [ ] Discover and record network connections.
	- [ ] Report connections to the team leader for the network inventory.
- [ ] Discover and record running services.
	- [ ] Test scored services and **fix** as necessary.
	- [ ] **Disable** services which are not scored &mdash; ensure they are not scored indirectly!
- [ ] Check running processes for suspicious activity or unneeded permissions.
- [ ] Discover all existing administrative accounts.
	- [ ] **Disable** administrative access for all unused accounts.
- [ ] Discover all existing user accounts.
	- [ ] **Disable** (not delete!) all unused accounts.
- [ ] Discover listening ports (e.g. `ss -lnptu`).
	- [ ] **Close** unused ports.
- [ ] Discover current host firewall configuration.
	- [ ] Change configuration to minimize attack surface, including egress rules.
- [ ] Secure (harden) scored services.
- [ ] Install and configure network monitoring.


## Per-machine information

- [ ] Which machine (name, piece of hardware)?
- [ ] What OS (version, patch number, etc)?
- [ ] Network hardware (NICs, WiFi, BT, etc)?
- [ ] Physically connected networks?
- [ ] Host IP addresses?
- [ ] Mapped IP addresses?
- [ ] Scored services running?
- [ ] Required services running?
- [ ] Implicitly required services running?
- [ ] Other services running? (Why not stop them?)
- [ ] Sensitive information stored here?
- [ ] Known vulnerabilities?
- [ ] Possible mitigations?

https://www.cvedetails.com/