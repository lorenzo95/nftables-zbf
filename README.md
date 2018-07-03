# nftables-zbf
nftables Zone-based Firewall. Tested with nftables v0.8.2. Comes with 18.04


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



