## Extremely Lightweight DD-WRT Blocklist

This is an **extremely small** list of advertising and analytic domains for blocking in DD-WRT routers. The list is in DNSMasq format.

The intention of this list is to block only the abolsute most common ad servers by domain. 

In my experience the Google network of advertising content distribution are the most common providers of ads on the Internet (*doubleclick.net*, *googleadservices.com*, and *googlesyndication.com*). These domains, with typical Internet usage, likely top the list of the highest number of DNS requests coming from your network. Solely blocking these three domains will likely result in a significant decrease in the number of ads you experience online.

This list is for users who don't want to attempt to block all ads at the router-level, but feel they might as well block the absolute most common.
### Installation

Copy the contents of **list.txt** into 'Additional DNSMasq Options' under 'Services>Services>DNSMasq' in the DD-WRT control Panel.

Make sure DNSMasq is enabled, and client devices are getting **only** the router's IP address via DHCP for DNS.
