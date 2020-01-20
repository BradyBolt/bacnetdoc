# BACnet Documentation (the search continues...)

**Notice: any and all of these resources can be found online freely. Since it's not my intention to link to material explicitly from *ANSI/ASHRAE 135: The BACnet Standard* let me know if any of these sources need to be taken down**

Good BACnet resources are like an oasis in the Sahara. Hopefully a list of pointers could help somebody some-what. In general when researching weird topics, a couple things to do include:

* Q: Who's famous/well known in this area? Why? What stuff have they done or made?
	- [BACnet Bill](http://www.bacnet.org/DL-Docs/Swan-in-Memoriam.html): nurtured BACnet since its infancy. Check out his [blog](https://bacnetbill.blogspot.com/). 
	- [Mr. Steve Karg](https://steve.kargs.net/bacnet-consulting/): implemented one of the most widely used BACnet stacks in the industry: [BACnet Stack](http://bacnet.sourceforge.net/), and has touched almost everything you'll probably run into as a BACnet developer.
	- *Note:* BACnet developers are often referred to as BACneteers.
* Q: What tools would I need?
	- YABE: some frustrated dude made is own BACnet explorer. Most use this today.
	- VTS: A go-to, especially before YABE, for exploring, testing, and interacting with BACnet devices.
		+ Heads up: VTS supports scripts (although with a unique syntax)
	- WireShark: An indispensable tool for prying incoming packets to interrogate your devices for debug info. The application knows the BACnet protocol due to the efforts of Karg.
