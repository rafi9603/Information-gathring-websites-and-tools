
###WEB SITES TO START RECON
***
##1.Shodan.io
Shodan is a search engine that lets the user find specific types of computers.
(webcams, routers, servers, etc.) connected to the internet using a variety of filters.
Some have also described it as a search engine of service banners,
which are metadata that the server sends back to the client.

##2.Censys.io
Censys is a platform that helps information security practitioners discover, monitor, 
and analyze devices that are accessible from the Internet.
Enterprises use Censys to understand their network attack surfaces.
CERTs(community emergency response teams) and security researchers, 
use it to discover new threats and assess their global impact.

##3.Crt.sh
crt.sh is a web interface to a distributed database called the certificate transparency logs.
certificate-transparency.org CRT is a file extension for a digital certificate file used with a web browser.
CRT files are used to verify a secure website's authenticity,
distributed by certificate authority (CA) companies such as GlobalSign, VeriSign and Thawte.

##4.Archieve.org
It provides free public access to collections of digitized materials,
including websites, software applications/games, music, movies/videos, moving images, and millions of books.
In addition to its archiving function, the Archive is an activist organization, advocating a free and open Internet.

##5.Mxtoolbox.com
MxToolbox detects the IP addresses those services are actively using to send your messages and if they are blacklisted.
You can even view your sender's reputation via MxRep to gauge how well their services are functioning.
MxToolbox supports global Internet operations by providing free, fast and accurate network diagnostic and lookup tools.
Millions of technology professionals use this tools to help diagnose and resolve a wide range of infrastructure issues.

##6.Kitterman.com
These tools are meant to help you deploy SPF records for your domain.
They use an actual RFC 7208 compliant library (pyspf) for tests and will dynamically test for processing limit errors (no other testers I'm aware of do this).
This site uses a caching DNS resolver, so for tests that use live DNS, results will be cached for the Time To Live of the DNS record. For most basic uses,
these tests should be reasonably self explanatory. Advanced users may need, and probably want.

##7.Greynoise.io
The data GreyNoise collects can be used to ignore traffic from omnidirectional background scanners,
allowing you to focus on targeted scan and attack traffic.
You can use the data to track opportunistic botnets that are comprised of compromised IOT devices.
You can use the data to stay informed of what kinds of software people are scanning for.

##8.Hunter.io
Hunter is an email finder and email verifier tool which allows you to perform domain search for email addresses.
Launched in 2015 by Francoise Grante As mentioned by François Grante (founder of the software),
Hunter.io works by searching and indexing emails it finds on company websites across the internet.
For email addresses it finds, Hunter.io will log the common email patterns and apply that logic to websites its users are searching.

##9.Recon.dev
Recon. Dev  is to build easy to use tools for bug bounty hunters to easily discover and assess targets in the cloud at scale.
They collect detailed domain to IP mappings of nearly 88+ Million IP addresses across all major cloud providers.
along with aggregated CIDR ranges for major bug bounty targets.
resulting in a data set of over 1 Million bounty eligible targets updated every Monday and easily searchable through our API.

##10Spider foot.net(OSINT)
With almost 200 modules and growing, SpiderFoot provides an easy-to-use interface that enables you to automatically
collect Open Source Intelligence (OSINT)(Open-source intelligence) about IP addresses,
domain names, e-mail addresses, usernames, names, subnets and ASNs from many sources such as AlienVault,
HaveIBeenPwned, SecurityTrails, SHODAN and more.
In Investigations you Found a suspicious IP address in your logs or received a targeted phishing attempt?
Perhaps you want to dig deeper into the e-mail address used, or links referenced? SpiderFoot HX provides an intuitive graph-based interface,
enabling you to incrementally investigate such entities to pin-point the information you’re seeking.

###TOOLS - FETCHING TARGET INFORMATION WITH OUT TOUCHING TARGET

##1.Dig tool (Domain information groper)
Dig is a network administration command-line tool for querying Domain Name System (DNS) name servers for information about host address.
It is useful for verifying and troubleshooting,DNS problems and also to perform DNS lookups and displays the answers.
that are returned from the name server that were queried.

**
Dig command:-

             dig bmw.com
             
             dig hotstar.com


##2.Nmap tool (Network Mapper) 
Nmap is now one of the core tools used by network administrators to map their networks.
The program can be used to find live hosts on a network, perform port scanning, ping sweeps, OS detection, and version detection.

**

Nmap command:-

            nmap -sT target ip      Scan using TCP connect


            nmap -sS target ip      Scan using TCP SYN scan	

If you want to know more commands visit this web site https://www.yeahhub.com/top-30-basic-nmap-commands-beginners/

##3.Amass tool
Amass is an open source network mapping and attack surface discovery tool that uses information gathering and other techniques,
such as active reconnaissance and external asset discovery to scrap all the available data.This tool maintains a strong focus on DNS,
HTTP and SSL/TLS data discovering and scrapping.

**

amass command:-

              amass intel -d owasp.org -whois     for finding subdomains

If you want to know more commands visit this web site https://medium.com/@hakluke/haklukes-guide-to-amass-how-to-use-amass-more-effectively-for-bug-bounties-7c37570b83f7


##4.Aquatone tool
AQUATONE is a set of tools for performing reconnaissance on domain names.
It can discover subdomains on a given domain by using open sources as well as the more common subdomain dictionary brute force approach.

**
Aquatone command:-

                 aquatone-discover --domain example.com  

If you want to know more commands visit this web site https://www.programmersought.com/article/1372240756/

##5.Sublist3r tool
Sublister is a tool designed in python and uses OSINT (Open-source intelligence) in order to enumerate subdomains of websites.
It helps pen-testers in collecting and gathering subdomains for a domain which is their target.

**
sublist3r command:-

                  python sublist3r.py -d google.com   

##6.Gobuster tool
Gobuster is a tool used to brute-force: URIs (directories and files) in web sites. DNS subdomains (with wildcard support).

**

  gobuster command:-     
                           finding flies/directories  
                           --------------------------
                    Type: gobuster dir -u http://192.168.1.105/dvwa -w /usr/share/wordlists/dirb/common.txt

                          -u is used to assign target URL, 192.168.1.105 is our target/DVWA.
                          -w is used to assign wordlist. /usr/share/wordlists/dirb/common.txt is the wordlist location.

 If you wnat to know more commands visit this web site https://www.securitynewspaper.com/2019/11/04/bruteforce-any-website-with-gobuster-step-by-step-guide/

