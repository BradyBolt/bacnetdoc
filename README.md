# BACnet Documentation (the search continues...)

**Notice: any and all of these resources can be found online freely. Since it's not my intention to link to material explicitly from *ANSI/ASHRAE 135: The BACnet Standard* let me know if any of these sources need to be taken down**

Introduction
============

A collection of decent BACnet resources for noobs like myself.

Getting Started
===============

What is BACnet?
---------------

The official name is ANSI/ASHRAE 135-XXXX, BACnet (TM) (where `XXXX`
denotes some yearly standard, 1995, 2016, 2019, and so on). It's what
HVAC people decided their machines will communicate with. A lot of the
material you read will not entirely make sense without basic
networking knowledge ([etc](https://support.microsoft.com/en-us/help/164015/understanding-tcp-ip-addressing-and-subnetting-basics)). Also, when it doubt [go to the
source](https://blog.codinghorror.com/learn-to-read-the-source-luke/).

BACnet is merely a protocol, so there's a lot of leg-room and user-freedom (i.e. 'work') for the developer that's involved in setting up a BACnet system. There is a [bible](https://www.techstreet.com/standards/ashrae-135-1-2019?product_id=2082781) that comes out with new editions (with a [official guide](http://www.momentumpress.net/books/bacnet-global-standard-building-automation-and-control-networks)
to go with it).

Background Info
---------------

* Q: Who's famous/well known in this area? Why? What stuff have they done or made?
	- [BACnet Bill](http://www.bacnet.org/DL-Docs/Swan-in-Memoriam.html): nurtured BACnet since its infancy. Check out his [blog](https://bacnetbill.blogspot.com/). Dedicated each year through the *Swan Award* as part of the annual [Plug-fest](https://www.bacnetinternational.org/page/plugfest) event.
	- [Mr. Steve Karg](https://steve.kargs.net/bacnet-consulting/): responsible for a widely used BACnet stack implementation: [BACnet Stack](http://bacnet.sourceforge.net/) and is a good authority on the BACnet standard in general
	- Mike Newman: The guy who made BACnet
	- Other important people in [this video](https://www.youtube.com/watch?v=Jzs-Q_blwN0&feature=youtu.be)
	- *Note:* BACnet developers are often referred to as BACneteers.
* Q: What tools would I need?
	- [YABE](https://sourceforge.net/projects/yetanotherbacnetexplorer/): some frustrated dude made his own BACnet explorer. Most use this today.
	- [VTS](http://vts.sourceforge.net/): A go-to, especially before YABE, for exploring, testing, and interacting with BACnet devices.
		+ Heads up: VTS supports scripts (although with a unique syntax)
		+ VTS has really good documentation
	- WireShark: An indispensable tool for prying incoming packets to interrogate your devices for debug info. The application knows the BACnet protocol due to the efforts of Karg.
	- Chipkin's Explorer: their utility was one of the reasons why YABE exists (*not in a good way*). But the good thing that came out of this was their wonderful documentation! Seriously, there are good nuggets of information in their [articles](https://store.chipkin.com/articles/) (their [BACnet index page](https://store.chipkin.com/articles/bacnet-index-page))
		+ It's also worth checking out their [manuals page](https://store.chipkin.com/articles/manuals-index-page)
	- BACnet Programming
		+ Stack Implementations
			* Python: The [bacpypes](https://github.com/JoelBender/bacpypes) stack is exposed by the nice and simple [BAC0 interface](https://github.com/ChristianTremblay/BAC0)
			* C: Karg's [BACnet Protocol Stack](https://sourceforge.net/projects/bacnet/) for C is time-tested and widely used
			* Java: [Bacnet4J](https://github.com/infiniteautomation/BACnet4J) supporting BACnetIP over ivp4 and ivp6 as well as MS/TP
			* C#: [BACsharp](https://sourceforge.net/projects/bacsharp/) stack
	- Karg talks about many other [useful tools out there](http://bacnet.sourceforge.net/) being used for BACnet and is definitely worth checking out  

Reading
-------

[Read this first](https://buildingautomationmonthly.com/definitive-guide-bacnet/), and [see this for a more formal but gentle introduction](https://www.ccontrols.com/pdf/BACnetIntroduction.pdf) (there's [more here](https://www.ccontrols.com/lc/index.htm) you might find relevant like material on MODBUS). Then work through the following below in any order:

- Building on the first reading, Chipkin provides their own very nice [introductory resource](https://c3.chipkin.com/assets/uploads/2018/mar/15-19-09-42_Bacnet_For_Beginners2.pdf) that includes much more material
- Another great resource to check out is the [BACnet Ontology](http://bacowl.sourceforge.net/index.html) project
- An older write-up done by BACnet Bill covering [The Language of BACnet](http://www.bacnet.org/Bibliography/ES-7-96/ES-7-96.htm) provides a condensed synthesis of the important bits you just read above
- [BACnet MS/TP Server Driver Manual](http://www.iccdesigns.com/products/millennium/documents/BACnet%20MS%20TP%20Server.pdf): besides being vendor user's manual, this resource covers a number of useful definitions for different BACnet properties and objects (this is useful to look at while looking at the previous resource)
- [BACnet Basics](https://dms.hvacpartners.com/docs/1000/Public/04/11-808-417-01.pdf): a vendor user-guide to skim quickly over to get an idea of how the first reading applies in action (but probably not as helpful as the other resources)
- [BBMD Utility User Guide](https://dms.hvacpartners.com/docs/1000/public/05/11-808-511-01.pdf): it's a good idea to look at this to get an idea of how BACnets are configured to find each other
- [BAMTV 005: BACnet Integration Fundamentals part 1](https://www.youtube.com/watch?v=uhjbEoktMAk&feature=youtu.be): BAMTV is all-around great for wrapping your head with BACnet
    - Do enough reading and discovery to *fully* understand everything the instructor goes over in this video
- More detailed info on the BACnet protocol can be found at [Understanding BACnet encoding](http://www.bacnet.org/Tutorial/Encoding.doc)
- The website [Automated Buildings](http://www.automatedbuildings.com) keeps their [articles over here](http://www.automatedbuildings.com/news/aug08/articles/)
- Steven Karg's directory of BACnet tutorials and write-ups can be found [here](http://kargs.net/BACnet/)
- Furthermore, you can find some other tutorials on the [BACnet website](http://www.bacnet.org/Tutorial/index.html) and checkout their [developer resources page](http://www.bacnet.org/Developer/index.html)

