# How does the internet work?

If you want to get to the bottom of every components of the internet the answer could be extremely long and complicated. There are books covering this topic with hundreds of pages. However, it could also be simplify as a map of connected servers. 


A common interview question what's the inner working of internet between a user type into a search engine then hit enter and the brower returns the content?

## Here is the work flow: 

1. when user hit enter, browser sent a packet which is an Http GET request to the server of the search engine. Packets follows TCP/IP protocol, it contains both user's query text and the location of server.
2. In order to send the packet to the server, IP address of the search engine need to be know. First, the browser cache and local DNS cache will be searched, if this search engine hasn't being used recently, a recursive DNS lookup will be conducted. (recursive here means it more take a couple different DNS servers to find the DNS  records of of the website and return the IP address.)
3. Once the browser has the IP address of the target server, browser will sent an ACK(acknowlegment) packet to server. Once server returns an ACK packet, the TCP connection between browser and search engine server is complete, the browser then send a HTTP requests to the server to retrieve the search result.   
4. These days, search engines usually have efficient API for handliing querys,  with thousnads of web crawlers and indexed database, content can be sent back to browser within a second. 
5. Established TCP connection signals browser to listening for incoming packets, for information usually splits into multiple packets. Then the Packets arrives, they will be displayed in the browser. 


## What's HTTP?
HTTP stands for Hyper text transfer Protocol. HTTP is a application layer protocol while TCP is a transport layer
Standard port: 80;
HTTPS port: 443;

## what is domain name? 
when you remember a website's name,what you remembered is its domain name. Domain name a string that identified one ore more IP addresses. 

## How does Web Browser work?
Web Browser hides details of HTTP protocols such as packets communication and provides user friendly content. 

## What is Hosting? 虚拟主机，网站托管是什么？
Hosting is the disk space, bandwidth, and tools used to create andmaintain a website. You can host your web site at your own PC, or most commonly, people would use web hosting services that owns large data centers. 




