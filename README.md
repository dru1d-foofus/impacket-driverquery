# impacket-driverquery
A modified version of wmiquery.py used for remote driver enumeration via WMI

I've been wanting a way to remotely query drivers on a target system to find candidates for driver exploitation, vulnerability research, and inventory.

This is my super hacky way of doing this using pre-existing code from impacket (https://github.com/fortra/impacket/blob/master/examples/wmiquery.py) and inspired by Matt's OffensiveCSharp DriverQuery tool (https://github.com/matterpreter/OffensiveCSharp/tree/master/DriverQuery).

It does not download drivers or check signing. It just spits out a .psv of all of the installed drivers on the endpoint; that's it.
