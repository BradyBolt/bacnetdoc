# BACnet Documentation (the search continues...)

**Notice: any and all of these resources can be found online freely. Since it's not my intention to link to material explicitly from *ANSI/ASHRAE 135: The BACnet Standard* let me know if any of these sources need to be taken down**

Introduction
============

Good BACnet resources are like an oasis in the Sahara. Hopefully a list of pointers could help somebody some-what. In general when researching weird topics, a couple things to do include:

PSA: I'm just an intern so don't expect everything to be correct.

Getting Started
===============

What is BACnet?
---------------

The official name is ANSI/ASHRAE 135-XXXX, BACnet (TM) (where `XXXX`
denotes some yearly standard, 1995, 2016, 2019, and so on). It's what
HVAC people decided their machines will communicate with. If somebody
hasn't told you this before: BACnet documentation isn't the greatest,
though there's a couple places to look at. A fair-warning, a lot of the
material you read will not entirely make sense without some basic
networking knowledge. Also, when it doubt [go to the
source](https://blog.codinghorror.com/learn-to-read-the-source-luke/).

More specifically, BACnet is merely a protocol. There is a
[bible](https://www.techstreet.com/standards/ashrae-135-1-2019?product_id=2082781)
that comes out with new editions (with a [traditional
guide](http://www.momentumpress.net/books/bacnet-global-standard-building-automation-and-control-networks)
to go with it).

Background Info
---------------

* Q: Who's famous/well known in this area? Why? What stuff have they done or made?
	- [BACnet Bill](http://www.bacnet.org/DL-Docs/Swan-in-Memoriam.html): nurtured BACnet since its infancy. Check out his [blog](https://bacnetbill.blogspot.com/). 
	- [Mr. Steve Karg](https://steve.kargs.net/bacnet-consulting/): implemented one of the most widely used BACnet stacks in the industry: [BACnet Stack](http://bacnet.sourceforge.net/), and has touched almost everything you'll probably run into as a BACnet developer.
	- *Note:* BACnet developers are often referred to as BACneteers.
* Q: What tools would I need?
	- [YABE](https://sourceforge.net/projects/yetanotherbacnetexplorer/): some frustrated dude made his own BACnet explorer. Most use this today.
	- [VTS](http://vts.sourceforge.net/): A go-to, especially before YABE, for exploring, testing, and interacting with BACnet devices.
		+ Heads up: VTS supports scripts (although with a unique syntax)
		+ VTS has really good documentation
	- WireShark: An indispensable tool for prying incoming packets to interrogate your devices for debug info. The application knows the BACnet protocol due to the efforts of Karg.
	- Chipkin's Explorer: their utility was one of the reasons why YABE exists (*not in a good way*). But the good thing that came out of this was their wonderful documentation! Seriously, there are good nuggets of information in their [articles](https://store.chipkin.com/articles/):
		+ Nugget 1
		+ Nugget 2

Reading
-------

Read/watch these in any order:

-   [BACnet
    Basics](https://dms.hvacpartners.com/docs/1000/Public/04/11-808-417-01.pdf)
-   [BBMD Utility User
    Guide](https://dms.hvacpartners.com/docs/1000/public/05/11-808-511-01.pdf)
    (it's a good idea to look at this to get an idea of how BACnets are
    configured to find each other)
-   [BAMTV 005: BACnet Integration Fundamentals part
    1](https://www.youtube.com/watch?v=uhjbEoktMAk&feature=youtu.be)
    (BAMTV is all-around great for wrapping your head with BACnet)
    -   Do enough reading and discovery to *fully* understand everything
        the instructor goes over in this video
    -   Once you're done with at least 005, reference [this
        resource](http://www.bacnet.org/Bibliography/ES-7-96/ES-7-96.htm)
        for more concrete examples of how BACnet objects are organized.
    -   If you're super hardcore, look at [Understanding BACnet
        encoding](http://www.bacnet.org/Tutorial/Encoding.doc)

