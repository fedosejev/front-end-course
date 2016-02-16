# Day 2

Questions:

1. [How does website work?](#how-does-website-work)
2. [What is URL (Uniform Resource Locator)?](#what-is-url-uniform-resource-locator)
3. [What is FQDN (Fully Qualified Domain Name)?](#what-is-fqdn-fully-qualified-domain-name)
4. [What is host name?](#what-is-host-name)
5. [What is localhost?](#what-is-localhost)
6. [What is Domain Name?](#what-is-domain-name)
7. [What is DNS (Domain Name Server)?](#what-is-dns-domain-name-server)
8. [What is IP address?](#what-is-an-ip-address)
9. [What is port number?](what-is-port-number)
10. [What are the different ways people access websites?](#what-are-the-different-ways-people-access-websites)
11. [What's the difference between web browsers?](#whats-the-difference-between-web-browsers)
12. [What's the most popular web browser today?](#whats-the-most-popular-web-browser-today)
13. [What's the most popular screen resolution today?](#whats-the-most-popular-screen-resolution-today)

Plus:

+ [Problems](problems.md)
+ [Guides](#guides)
+ [Tips and Tricks](#tips-and-tricks)
+ [Learn more](#learn-more)

## Questions

### How does website work?

+ [Digaram 1](http://2.bp.blogspot.com/-bdhI9VRD0l8/T7Wy-9v2NNI/AAAAAAAAAWY/2J5gk7zsY-E/s1600/Part+15_DNS.jpg)
+ [Article 1](https://ist.mit.edu/network/ip)

### What is URL (Uniform Resource Locator)?

> A URL (Uniform Resource Locator) is simply a URI (Uniform Resource Identifier) that happens to point to a physical resource over a network.
https://en.wikipedia.org/wiki/Uniform_Resource_Identifier#Conceptual_distinctions

+ URL syntax: https://en.wikipedia.org/wiki/Uniform_Resource_Locator#Syntax
+ URI syntax example: https://en.wikipedia.org/wiki/Uniform_Resource_Identifier#Examples

Example of a URL: `http://maps.google.com:80`

1. Scheme: `http` - uses `HyperText Transfer Protocol`.
2. Subdomain name/machine name/host name: `maps`.
3. Domain name: `google.com`.
4. Port number: `80`.

> The __domain name__ would reach you to the campus network and the __host name__ would let you reach the exact machine in the campus.
http://superuser.com/a/59094

#### Warning!

`scheme` is __NOT__ `protocol`

> Some URI schemes are not associated with any specific protocol (e.g. `file`) and many others do not use the name of a protocol as their prefix (e.g. `news`).
https://en.wikipedia.org/wiki/Uniform_Resource_Identifier#Conceptual_distinctions

### What is FQDN (Fully Qualified Domain Name)?

> A fully qualified domain name (FQDN) consists of the host name (including all subnames) and the domain name, including the top level domain (TLD).
https://ist.mit.edu/network/ip

Example: `map.google.com`

### What is host name?

> A host name is a name that is assigned to a host (i.e., a computer connected to the network) that uniquely identifies it on a LAN (local area network) and thus allows it to be addressed locally without using its full IP address. http://www.linfo.org/fqdn.html

Example: `map`

![](https://imgs.xkcd.com/comics/permanence.png)

### What is localhost?

`localhost` is a host name that means this computer or this host.

### What is Domain Name?

> A domain name is a name that uniquely identifies a site (e.g., web site or ftp site) on the Internet or other TCP/IP (Transmission Control Protocol/Internet Protocol) network. http://www.linfo.org/fqdn.html

Example: `google.com`

### What is DNS (Domain Name Server)?

Network of servers that map domain name to IP address.

+ [Article 2](http://amar-linux.blogspot.co.uk/2012/05/how-dns-works.html)
+ A fun and colorful explanation of how DNS works: https://howdns.works

### What is an IP address?

+ Each device connected to the Internet has a unique IP address.
+ It's a number.
+ `IPv4`: up to 12 digits, e.g.: `192.168.0.1` - a total of __4,294,967,296__ unique IP addresses.
+ `IPv6`: up to 32 characters, e.g.: `2002:4559:1FE2::4559:1FE2`

> `There are only 4.2×10^37 42 undecillion (sextillion) IPv6 addresses currently defined and usable.`
http://rednectar.net/2012/05/24/just-how-many-ipv6-addresses-are-there-really/

### What is port number?

> A port serves as an endpoint in an operating system for many types of communication. It is not a hardware device, but a logical construct that identifies a service or process.
https://en.wikipedia.org/wiki/Port_(computer_networking)

### What are the different ways people access websites?

+ Devices:
  + Servers
  + Desktops
  + Mobiles
  + Wearables
  + [Cars](http://www.popularmechanics.com/cars/a13191/the-future-of-car-connectivity-is-a-real-web-browser-in-the-dash-17416796/)
+ Software:
  + [Web Crawlers](https://www.google.co.uk/insidesearch/howsearchworks/crawling-indexing.html)
  + [Web Browsers](https://en.wikipedia.org/wiki/List_of_web_browsers#Notable_releases)
  + [Screen Readers](https://en.wikipedia.org/wiki/List_of_screen_readers)

### What's the difference between web browsers?

+ [Article 3](http://www.realtyninja.com/blog/whats-the-difference-between-browsers-and-why-do-people-think-internet-explorer-sucks/)

> The main difference between web browsers is a thing called a layout engine.
When you go to a webpage in a browser, the webpage gives your browser a set of ‘instructions’ (html, css, javascript, &c.) that tell the browser how the page should look & act when you interact with it. The browser interprets these instructions using its layout engine.
http://www.realtyninja.com/blog/whats-the-difference-between-browsers-and-why-do-people-think-internet-explorer-sucks/

---

> Microsoft has historically been very slow compared to the other browsers in implementing some of the newest changes to their layout engine.
http://www.realtyninja.com/blog/whats-the-difference-between-browsers-and-why-do-people-think-internet-explorer-sucks/

+ See a list of the most layout engines: https://en.wikipedia.org/wiki/List_of_web_browsers#Layout_engines
+ Check if your browser passes [Acid3](https://en.wikipedia.org/wiki/Acid3) test: http://acid3.acidtests.org/

### What's the most popular web browser today?

http://gs.statcounter.com/#all-browser-ww-monthly-201409-201509

### What's the most popular screen resolution today?

http://gs.statcounter.com/#resolution-ww-monthly-201409-201509

## [Problems](problems.md)

+ [Problem 1](problems.md#problem-1)
+ [Problem 2](problems.md#problem-2)
+ [Problem 3](problems.md#problem-3)
+ [Problem 4](problems.md#problem-4)
+ [Problem 5](problems.md#problem-5)
+ [Problem 6](problems.md#problem-6)
+ [Problem 7](problems.md#problem-7)
+ [Problem 8](problems.md#problem-8)
+ [Problem 9](problems.md#problem-9)
+ [Problem 10](problems.md#problem-10)
+ [Problem 11](problems.md#problem-11)
+ [Problem 12](problems.md#problem-12)
+ [Problem 13](problems.md#problem-13)
+ [Problem 14](problems.md#problem-14)
+ [Problem 15](problems.md#problem-15)

## Guides

### VoiceOver

To turn VoiceOver on OSX, use: `cmd` + `F5` and click `Use VoiceOver`.

To learn more about VoiceOver: https://www.apple.com/voiceover/info/guide/

Some organization required by law or other legal mandate to make its website accessible. See http://www.w3.org/WAI/bcase/pol#apply for more details.

## Tips and Tricks

### How to quickly find some text on a web page?

1. Press `cmd` + `f`.
2. Type the word you're looking for.
3. Press `Enter` to navigate through found words.
4. Press `esc` to exit search.

### How to find out what's my public IP address?

1. Google for `ip address`
2. In Terminal: `curl ipecho.net/plain && echo`

### How to find out what's my private IP address?

Open Terminal and type:

`ipconfig getifaddr en0`

### How to find out what `google.co.uk` IP address is?

1. In Terminal: `ping google.co.uk`
2. `cmd` + `c` to terminate.
3. See response: `PING google.co.uk (62.253.72.148): 56 data bytes`

### How to find out additional information about any domain name?

Use WHOIS lookup: https://who.is

### Given an image, how can I find all the websites that display this image?

Use Google image search: https://www.google.co.uk/imghp

## Learn more

1. Uniform Resource Identifier (URI): https://en.wikipedia.org/wiki/Uniform_Resource_Identifier
2. Uniform Resource Locator (URL): https://en.wikipedia.org/wiki/Uniform_Resource_Locator
3. IP Addresses, Host Names, and Domain Names: https://ist.mit.edu/network/ip
4. Fully Qualified Domain Name (FQDN): http://www.linfo.org/fqdn.html
5. List of web browsers: https://en.wikipedia.org/wiki/List_of_web_browsers#Notable_releases
6. List of layout engines: https://en.wikipedia.org/wiki/List_of_web_browsers#Layout_engines
7. List of screen readers: https://en.wikipedia.org/wiki/List_of_screen_readers
8. Google Bot: http://www.google.com/bot.html
9. How the Internet works: http://thumbnails-visually.netdna-ssl.com/how-the-internet-works_5391f01eeac65.jpg
10. IPv4: https://en.wikipedia.org/wiki/IPv4
11. IPv6: https://en.wikipedia.org/wiki/IPv6
12. Port number: https://en.wikipedia.org/wiki/Port_(computer_networking)
13. Application Ports: http://bandwidthcontroller.com/applicationPorts.html
14. Google image search: https://www.google.co.uk/imghp
15. WHOIS lookup: https://who.is
