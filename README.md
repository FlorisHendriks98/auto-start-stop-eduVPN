# Introduction
eduVPN is used to provide (large groups of) users a secure way to access the internet and their organisational resources. The goal of eduVPN is to replace typical closed-source VPNs with an open-source audited alternative that works seamlessly with an enterprise identity solution.

In order to establish an eduVPN connection with the default settings, the user has to run the eduVPN client and authenticate (if the previous VPN connection is expired). Sometimes the user tries to access the organisational resources without an established VPN connection. The user is then prompted with a generic error message and is confused why he or she can not access the resource. The user often then contacts the eduVPN support and the support tells the users to establish the VPN connection. These kind of trivial issues can cause unnecessary overhead for the eduVPN support team.  

The Windows eduVPN developer has partially mitigated this limitation by offering the option to start eduVPN on sign-on. As long as the VPN configuration has not expired, the eduVPN client is able to establish the VPN connection automatically. However, this option is not offered by default. Moreover, if one enables this option for every VPN user the amount of concurrent VPN users can increase tremendously, as the VPN is on most of the time.

We therefore need to find a way in order to automatically start and stop eduVPN so that we minimalize the number of support requests that are related to forgetting to establish the VPN connection, and we minimalize unnecessary overhead of the eduVPN server.

