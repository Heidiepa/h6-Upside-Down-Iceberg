# h6-Upside-Down-Iceberg

h6 Upside Down Iceberg
In Finland, it's legal to use TOR at the time of writing. If you reside in another juristiction, laws might be different. Obviously, it's illegal to do illegal things in TOR, just like it's illegal to do illegal things anywhere. Only do legal things.

If you reside in a jurisdiction where using TOR is illegal, you obviously can't install it and do the related tasks. If you cannot or do not want to do the hands-on darknet tasks, the alternative task is: based on literature only (no hands on tests, no installation), compare anonymous/pseudonymous networks, such as TOR, I2P, Freenet and others. How do their goals, technology and other features differ? How are they similar? Add references. Link differences and benefits to technical and architecture aspects.

## Read and summarize (briefly, e.g. with some bullets)
### Dingledine, Mathewson and Syverson 2004: Tor: The second-generation onion router. In USENIX security symposium (jufo level 2). Chapter:
3 Design goals and assumptions

### Karunanayake, Ahmed, Malaney, Islam and Jha 2021: De-anonymisation attacks on tor: A survey. In IEEE Communications Surveys & Tutorials (jufo level 2). Chapters:
Abstract
I Introduction
II Background (to the end of "B. Circuit Establishent for Tor HS")
Fig. 6. Taxonomy for Tor attacks (Just the figure on page 2330.)

### Halonen, Ollikainen, Rajala 2023: PhishSticks - The Ethical Hackers tool for BadUSB (Video, about 3 minutes)


## Practical exerises
### a) Install TOR browser and access TOR network (.onion addresses). (Explain in detail how you installed it, and how you got access to TOR).

I approached the exersize in following manner:
1. Google "TOR browser"
2. Selected the first one, seemed to be reliable with onions
   ![image](https://github.com/user-attachments/assets/68a9e53e-9ba5-41bd-b86e-1f2bb90bdc3f)
3. Installed Windows version
4. ![image](https://github.com/user-attachments/assets/c3fad87d-41f5-4534-80e9-b1c44fca0ad0)
5. Connected to the network
   ![image](https://github.com/user-attachments/assets/9dd596a6-5bb0-46aa-836a-ecabd7936a3a)

To be honest, I was bit hesitant to install Tor browesr and access TOR network due to legal complications (I'm lawful neutral) but apparently it is not illegal in Finland to access TOR network. In Venezela this homework would not be OK, thanks NordVPN. https://nordvpn.com/fi/blog/tor-selain/

### b) Browse TOR network.
Find, take screenshots and comment
* search engine for onion site: Is DuckDuckGo which is more secure version of Google Chrome. DuckDuckGo does not track its users nor does it store any data about user searches.
![image](https://github.com/user-attachments/assets/78d7cad1-3922-478b-89cc-9ee31d400f78)

human rights or civil rights organization: DuckduckGo hides the search query
![image](https://github.com/user-attachments/assets/d4354378-04ef-49e2-9bb7-f085ea9e8f57)

marketplace: I presume this task was supposed to be about accessing TOR web marketplace. I somehow feel that I'm not supposed do to that (again, moral compass too strong) so I searched just normal marketplaces
![image](https://github.com/user-attachments/assets/e9ad46bd-2fcd-4689-9f85-ffdf515b9000)

fraud: Found normal results  of fraud
![image](https://github.com/user-attachments/assets/36aa25ec-1cb1-4b8b-aa6f-b6ebf6370cfa)

forum: Seacrhed for forum and got prevented from accessing.
![image](https://github.com/user-attachments/assets/e73c84e7-3736-4244-b824-fc6294decd06)

a well known organization (with regular postal addresses, offices or similar presence outside darknet): I searched for Posti.fi and found their address site.
![image](https://github.com/user-attachments/assets/0c4b5280-0c27-40a4-a38a-74a0c1bbbb31)


Use .onion addresses inside TOR network, not regular (clearnet) websites trough exit nodes.


### c) Onion. In your own words, how does anonymity work in TOR? (e.g. how does it use: public keys, encryption, what algorithms? This subtask does not require tests with a computer.)

So, you probably known the movie Shrek. Tor and Shrek (the titular character of the movie) have something in common and that is layers. Like onions. When connecting to Tor network, one's PC connects one computer in Tor network which then connects to next computer in the network and then eventually to the server. Because there are so many connections, server does not relaize it is your computer that is connecting to it, it is some other computer. This is why TOR is very anonymous. Ogres are not that anonymous so in that sense TOR is not like Ogre but kinda is.

![image](https://github.com/user-attachments/assets/99927e5a-9a51-48cf-b86a-52f04076d6bf)

To provide highest level of anonymity, Tor network utilizes many cybe security concepts. All Tor connections are done via Transport Layer Security (TLS) protocol that is used to enable secure connections through internet. There is also encruption in each layer of Tor-Onion to ensure best security levels. Tor uses public keys to ensure high quality authentication. They are called onion keys. Onion keys are rotated between layers



### d) What kind of the threat models could TOR fit? (This subtask does not require tests with a computer.)

### e) Don't stick that stick. How does PhishSticks attack work? Would a typical organization be vulnerable? Does this link to a broader category of attacks and defenses? How could the risk be mitigated? (This subtask does not require tests with a computer.) (If you want, you can view PhishSticks on Github and PhishSticks Youtube channel.

## Sources
Tell me about all the keys Tor uses
https://support.torproject.org/about/key-management/ 

