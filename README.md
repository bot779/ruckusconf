ruckusconf
==========

negotiate ssh login.
Automate config downloads, script execution, config changes, etc.

Usage: ruckusconf \[OPTIONS\] device_ip\n
Options:
--username <username>
--password <passw0rd> ;# not recommended or "safe"
--enable  ;# bring the ruckus to enable mode
--config  ;# bring the ruckus to config mode
--debug   ;# bring the ruckus to debug mode
--script  ;# bring the ruckus to script mode
--section <context> ;# change to configuration-context mode
--exit    ;# exit out of configuration-context mode
--ap      ;# connect to an access point (not a controller)
--command <command line> ;# run the command in the specified mode
--timeout <seconds>      ;# set the timeout for the next command
--waittime <seconds>     ;# time to wait before beginning the timeout interval
--quiet                  ;# suppress command output
--outfile <save/output/in/filename>
--infile <read/rules/from/filename>
--makeinfile <write/rules/to/filename>
--devlist <read/device_ip/list/from/filename>
--localdebug ;# show internal debugging info from the ruckusconf script
--example ;# show examples and exit


--------------------------------

buildclientos.txt
=================

Use ruckusconf to:
build an inventory of wireless clients showing the operating system of each client.
store this "database" in the clientos.txt file.
results are cumulative.
running this command adds to the clientos.txt file.
