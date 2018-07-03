# nftables-zbf
nftables Zone-based Firewall. Tested with nftables v0.8.2. Comes with 18.04

	- Currently just a framework. Not to be considered secure -


		Default Permitted Packet Flow

		   +-------+
			   |
			   |
	  +----------+     v  +--------+
	  |          |                 |
	  |          |                 |
	  |          +-----------+     v  +-------+
	  |          |           |                |
	  |          |           |                |
	  | Inside / |           +-----------+    v
	  |   VPN    |           |           |
	  |          |   DMZ     |           |
	  |          |           |    IoT    +-----------+
	  |          |           |           |           |
	  |          |           |           |  Outside  |
	  |          |           |           |           |
	  +----------------------------------------------+
			    ^                      +
			    |                      |
			    +----------------------+
			       Reverse Proxy dnat



