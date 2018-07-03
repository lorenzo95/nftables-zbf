# nftables-zbf
nftables Zone-based Firewall. Tested with nftables 0.9. 


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



