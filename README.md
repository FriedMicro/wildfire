# Wildfire
A lightweight wrapper for Linux iptables

This script is intended to be used for http servers. Its goal is to provide a extremely lightweight solution for management of network traffic without adding extra daemons or user-space programs on the machine if the machine does not need automated network traffic manipulation

Commands:

-flush: wipe the iptables config for everything minus ssh, http, and https; this will not disconnect the user

-help: Display an abreviated version of all command documentation

-get: List the current configuration in iptables

-ban: Ban the ip; takes ip to ban as a param

-save: Save the iptables configuration

-drop: Remove a saved rule from iptables (do remember to run save)

-open-port: Opens the specified port; syntax is wildfire -open-port port_number port_type

Entering an invalid command will cause the program to send all possible commands back to a user
