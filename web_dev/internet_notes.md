# the Complexities of the Internet 

## Domain Name System (DNS)

- The internet is addressed through IP (Internet Protocol) and the DNS serves as a sort of Yellow Pages for the internet.

- All webpages have a unique IP address, and the Domain Name System is like an address book that matches domain name to IP address.

- When a URL is typed into your browser, your machine sends a out a DNS request to locate the corresponding IP address.


<p align="center">
  <img src="https://sw.nohold.net/CiscoSB/Images/3775_1.png">
</p>



## Steps of a DNS Lookup

- When you enter a URL into your web browser, the DNS request will first be sent to a recursive name server. The recursive name server is typically operated by your ISP (internet service provider).
- A recursive name server would be like a phone operator looking into a phone book on behalf of the requesting party. Further, in the recursive case, last names have a seperate phone book and first names have another phone book, making the process categoristically recursive. 