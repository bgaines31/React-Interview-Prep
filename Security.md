<li><b> cross-site scripting (XSS)</b> XSS is a type of “attack”, in which malicious code is injected into otherwise trusted websites.

The end user’s browser, unaware of any trickery, will execute the script. The malicious script will gain access to cookies, session tokens, or any other sensitive information retained by the browser. There are various types of attack, including reflected, stored, and DOM-based XSS. Attacks can be prevented by sanitizing input, encoding output and using appropriate response headers.
To keep yourself safe from XSS, you must sanitize your input. Your application code should never output data received as input directly to the browser without checking it for malicious code.

The simplest way of cross-site scripting vulnerability elimination would be to pass all external data through some filter. Such a filter would remove dangerous keywords, for example, the infamous <code>script</code> tag, JavaScript commands, CSS styles, and other dangerous HTML markups (such as those that contain event handlers).
</li>
<li><b>What is HTTPS? </b>HTTPS stands for Hypertext Transfer Protocol Secure. It is an encrypted version of HTTP (Hypertext Transfer Protocol). This means that sensitive data like passwords cannot be read while in transit. Any website, especially those that require login credentials, should use HTTPS. In modern web browsers such as Chrome, websites that do not use HTTPS are marked differently than those that do.</li>
<li><b>What is a SQL Injection? And how to mitigate the SQL Injection risks? </b>It’s a type of attack when a piece of SQL code is injected into the input field. For instance, if you have a search form where a user types in a name like “John”, you take that string and do an SQL lookup for it. Let’s say your SQL looks like this:
<code>SELECT * FROM Users WHERE UserName = valueFromSearch</code>
An attacker could put something malicious in the search bar like John OR 1=1, and now it will return a list of all users instead of just the requested one.

Most instances of SQL injection can be prevented by using parameterized queries (also known as prepared statements) instead of string concatenation within the query.</li>
<li><b>CORS: </b>Cross-Origin Resource Sharing (CORS) is an HTTP-header-based mechanism that allows a server to indicate any origins (domain, scheme, or port) other than its own from which a browser should permit loading resources. CORS also relies on a mechanism by which browsers make a “preflight” request to the server hosting the cross-origin resource, in order to check that the server will permit the actual request. In that preflight, the browser sends headers that indicate the HTTP method and headers that will be used in the actual request.</li>
<li><b>What is a Firewall? </b>It is a security system designed for the network. A firewall is set on the boundaries of any system or network which monitors and controls network traffic. Firewalls are mostly used to protect the system or network from malware, worms, and viruses. Firewalls can also prevent content filtering and remote access.</li>
<li><b>How would you explain SSL? </b>SSL stands for Secure Sockets Layer. It is a technology creating encrypted connections between a web server and a web browser. It is used to protect the information in online transactions and digital payments to maintain data privacy.</li>
<li><b> brute force attack: </b>It is a trial-and-error method to find out the right password or PIN. Hackers repetitively try all the combinations of credentials. In many cases, brute force attacks are automated where the software automatically works to log in with credentials. </li>
<li><b>man-in-the-middle attack: </b>The criminal sniffs sensitive traffic to identify the victim's session token. With that information, the attacker uses source-routed IP packets to intercept data as it's being transferred from the victim's computer to the server and make requests as though they were the user</li>
<li><b>cryptography: </b>Cryptography is technique of securing information and communications through use of codes so that only those person for whom the information is intended can understand it and process it. Thus preventing unauthorized access to information. The prefix “crypt” means “hidden” and suffix “graphy” means “writing”. In Cryptography the techniques which are use to protect information are obtained from mathematical concepts and a set of rule based calculations known as algorithms to convert messages in ways that make it hard to decode it. These algorithms are used for cryptographic key generation, digital signing, verification to protect data privacy, web browsing on internet and to protect confidential transactions such as credit card and debit card transactions. </li>
<li><b>What is the difference between a threat, a vulnerability, and a risk?</b> A vulnerability is a flaw or weakness in an asset's design, implementation, or operation and management that could be exploited by a threat. A threat is a potential for a threat agent to exploit a vulnerability. A risk is the potential for loss when the threat happens.</li>
<li><b>three-way handshake: </b>A three-way handshake is a method used in a TCP/IP network to create a connection between a local host/client and server.
It is a three-step method designed to allow both communicating ends to initiate and negotiate the parameters of the network TCP socket connection at the same time before data such as HTTP and SSH is transmitted.
Multiple TCP socket connections can be transmitted in both directions simultaneously. A three-way handshake is also known as a TCP handshake or SYN-SYN-ACK, and requires both the client and server to exchange SYN (synchronization) and ACK (acknowledgment) packets before actual data communication begins.</li>
<li><b>Encoding </b> ensures that data is formatted correctly so that it can be interpreted properly by applications and recipients. Think of it as data transformed into an easily read scheme to make communications possible.</li>
<li><b>Encryption</b> makes data unreadable to anybody except for the parties with the secret key used to decrypt the data. This makes it secret and secure and is used for securing data over private connections</li>
<li><b>Hashing</b> is a method that ensures that data integrity is maintained. A data hash is a string of data that is generated against the information that is being preserved. By generating a hash and comparing it to the original after transmission, you can verify that the data has not changed if the hashes match. If they don’t match, the information is no longer in its original state and should not be trusted.</li>
<li><b>CIA Triad: </b> 
<ul>
<li><b>Confidentiality:</b>keeping data hidden and private from the outside world</li>
<li><b> Integrity:</b> data has not been manipulated or otherwise changed. Commonly enforced by using identity access management tools and methods</li>
<li><b>Availability: </b>accessibility of data for approved users</li>
</ul>
<li><b> How is Encryption different from Hashing?</b> Both Encryption and Hashing are used to convert readable data into an unreadable format. The difference is that the encrypted data can be converted back to original data by the process of decryption but the hashed data cannot be converted back to original data.</li>
<li><b>Vulnerability Assessment</b> is the process of finding flaws on the target. Here, the organization knows that their system/network has flaws or weaknesses and want to find these flaws and prioritize the flaws for fixing.</li>
<li><b>Penetration Testing</b> is the process of finding vulnerabilities on the target. In this case, the organization would have set up all the security measures they could think of and would want to test if there is any other way that their system/network can be hacked.</li>
<li><b>Response codes from a Web Application</b>
<ul>
<li><b>1xx – </b>Informational responses</li>
<li><b>2xx – </b>Success</li>
<li><b>3xx – </b>Redirection</li>
<li><b>4xx – </b>Client-side error</li>
<li><b>5xx – </b>Server-side error</li>
</ul>
</li>
<li><b>Traceroute</b> is a tool that shows the path of a packet. It lists all the points (mainly routers) that the packet passes through. This is used mostly when the packet is not reaching its destination. Traceroute is used to check where the connection stops or breaks to identify the point of failure.</li>
<li><b>Data Leakage: </b>Data Leakage is an intentional or unintentional transmission of data from within the organization to an external unauthorized destination. It is the disclosure of confidential information to an unauthorized entity. Data Leakage can be prevented by using tools, software, and strategies known as DLP(Data Leakage Prevention) Tools
 Data Leakage can be divided into 3 categories based on how it happens:
<ul>
<li><b>Accidental Breach: </b>An entity unintentionally send data to an unauthorized person due to a fault or a blunder</li>
<li><b>Intentional Breach: </b>The authorized entity sends data to an unauthorized entity on purpose</li>
<li><b>System Hack:</b> Hacking techniques are used to cause data leakage</li>
</ul>
</li>
<li><b>VPN: </b>VPN stands for Virtual Private Network. It is used to create a safe and encrypted connection. When you use a VPN, the data from the client is sent to a point in the VPN where it is encrypted and then sent through the internet to another point. At this point, the data is decrypted and sent to the server. When the server sends a response, the response is sent to a point in the VPN where it is encrypted and this encrypted data is sent to another point in the VPN where it is decrypted. And finally, the decrypted data is sent to the client. The whole point of using a VPN is to ensure encrypted data transfer.</li>
<li><b>Black hat hackers</b> are known for having vast knowledge about breaking into computer networks. They can write malware which can be used to gain access to these systems. This type of hackers misuse their skills to steal information or use the hacked system for malicious purpose. </li>
<li><b>White hat hackers </b>use their powers for good deeds and so they are also called Ethical Hackers. Look out for our Ethical Hacking Course to learn more about the Ethical Hacking. These are mostly hired by companies as a security specialist that attempts to find and fix vulnerabilities and security holes in the systems. They use their skills to help make the security better. </li>
<li><b>Grey hat hackers</b> are an amalgamation of a white hat and black hat hacker. They look for system vulnerabilities without the owner’s permission. If they find any vulnerabilities, they report it to the owner. Unlike Black hat hackers, they do not exploit the vulnerabilities found. </li>
<li><b>DDOS attack </b> A DDOS(Distributed Denial of Service) attack is a cyberattack that causes the servers to refuse to provide services to genuine clients. DDOS attack can be classified into two types:
<ul>
<li><b>Flooding attacks: </b> In this type, the hacker sends a huge amount of traffic to the server which the server can not handle. And hence, the server stops functioning. This type of attack is usually executed by using automated programs that continuously send packets to the server.</li>
<li><b>Crash attacks: </b> In this type, the hackers exploit a bug on the server resulting in the system to crash and hence the server is not able to provide service to the clients.</li>
</ul>
</li>
<li><b>Cognitive Cybersecurity: </b>an application of AI technologies patterned on human thought processes to detect threats and protect physical and digital systems</li>
<li><b></b></li>
