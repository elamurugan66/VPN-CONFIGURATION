# VPN-CONFIGURATION
# VPN-Configuration-isakmp
Algorithm(Procedure):
***
Step 1:  Place 3 Routers(1941),2 PCs,1 Switch,1 Server  in the framework.
***
Step 2:  Connect the server with the switchand the IP address 192.168.2.254 is assigned to theserver.
***
Step 3:  Connect the PC1 with the switch with IP address 192.168.2.10.
***
Step 4:  Connect the Switch with the Main Router with IP address 192.168.2.1
***
Step 5:  Connect the Main Router with the Internet Router with Serial DCE(s0/0/1) cable with the IP 209.165.200.229
***
Step 6:  Connect the Internet Router with the Branch Router with Serial DCE(s0/0/0) cable with  IP 209.165.200.225
***
Step 7:  Connect the Branch Router with PC0 with IP 192.168.1.10 with Fa0.
***
Step 8:  Create an IProute 0.0.0.0 0.0.0.0 s0/0/0 in the Branch Router.
***
Step 9:  Create an IP access-list standard ACL_NAT permitting 192.168.1.0 with inside and outside.
***
Step 10: Configure the Main router with license boot module c1900 technology-package securityk9package.
***
Step 11: Set Local IP Pool of 192.168.2.100 to 192.168.2.115 and set the username as uservpn and the password ciscovpn using aaa authorization and crpyto isakmp policy 100, encryption aes 256,hash sha.
***
Step 12: Set the key as ciscogroupvpn.
***
Step 13: Click PC0 and in desktop click Vpn Configuration
***
Step 14: VPN DETAILS:
        GroupName: GroupVPN
        GroupKey:  ciscogroupvpn
        Host IP:   209.165.200.230
        UserName:  uservpn
        Password:  ciscovpn
