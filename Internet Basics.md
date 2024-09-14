Clients request information from other machines called servers,
every device has a unique identifier called IP address, human readable form of this identifier is called doamin name
every domain name is mapped to ip address through DNS (domain name system) ,
when you type domain name, browser contacts a DNS server which translates the domain into coressponding IP address

data is broken into several packets and those packets are sent across the internet, moving through various routers (guide the packets to their destination)
now these broken packets are aligned in order by TCP (transmission control protocol)/ IP (internet protocol),
TCP ensures that all packets have arrived and are in order and IP manages the addressing and routing

URL - Uniform Resource Locator :
it is a complete address to a specific source like a webpage or image 
(https://github.com/saddle-pt/Web-basics/blob/main/Internet%20Basics.md)
so it consists of several parts 
https or http is the protocol
www.example.com is the domain name 
/about is the exact location or the path of specific source


Entered URL is broken into components by browser : protocol , domain , path
Browser makes a request to DNS server to convert Domain name into IP address 
and once browser finally connects to the server it makes an HTTPS GET request to server hosting the IP address.

Now the browser establishes a TCP connection to the server on Port(a port is like a door from which the data flows in the server) 443 for HTTPS , if the server uses HTTPS then browser and server perform a TLS handshake to establish a secure connection by encrypting the data.

Server processes the request, retrieves necessary data and sends files back to browser

Run server-side code (if it's a dynamic site) to generate HTML dynamically, interact with databases, or process user data.
The server responds to the HTTP request by sending back the requested data, usually in the form of an HTTP response that includes:
Status code: Indicates whether the request was successful (like 200 OK), or if there was an error (like 404 Not Found).
Response headers: Meta information, such as the content type.
Response body: This is the actual content, like an HTML page, JSON data, or an image.

Browser takes this response and renders it (build and display these webpages )
html is parsed to structure page , css is applied , js is executed to handle interactions4

If website is dynamic , js would send more requests via API to load additional data without refreshing the page.
*** APIs are helpful in retrieving information from different servers , eg a weather website would provide data from the server that hosts it and the API ewould fetch live data from another server.




