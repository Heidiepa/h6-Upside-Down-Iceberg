# h6-Upside-Down-Iceberg

## Read and summarize (briefly, e.g. with some bullets)
### Dingledine, Mathewson and Syverson 2004: Tor: The second-generation onion router. In USENIX security symposium (jufo level 2). Chapter:
3 Design goals and assumptions

* Article explains the baseline for Tor network which is to prevent attackers from seeing linking network communication between two or more parties.
* Goals are clear. To ensure that goals are reached, Tor design must be inexpensive to built and manage, it must not be something attackers can claim as unlawful by design, it must be usable and simple to adopt and implement in all platforms (Windows, Linuz, Android, MacOS etc.). It also needs to be flexible in a sense that can be used to test and develop in the future. Finally, it has to have simple and easily understadbale design.
* Article also lists what Tor should not be. It should not be peer-to-peer because that approach poses risk if another peer is controlled by enemy. Tor is also not a solution for all possible issues: it does not conceal who is connected to network, it is not secure against end-to-end attacks


### Karunanayake, Ahmed, Malaney, Islam and Jha 2021: De-anonymisation attacks on tor: A survey. In IEEE Communications Surveys & Tutorials (jufo level 2). 

* The article about survey results that are used to investigate known risks of Tor network, including cyber security attacks and how to de-anonymise Tor users and hidden, possibly malicious services.
* Initially the article prefaces why internet user may prefer private connections. These are important for whistle-blowers, military, researcsh and business organisations and individuals that may want to preserve anonymity. Tor network is one of most known anonymous networks. While the idea of Tor is great, it is used by evil side of human nature: for cyber crime, terrorism and other criminal activities. The research analyses more than 30 tor de-anonymisation attacks to understand how to improve current practices and how to develop Tor in the future
*Second chapter describes how Tor network works, different components of Tor such as Onionisation, Directory servers (trusted server used for communication), nodes for entry and exit and how attack affect to those parts. Continuation is about how Tor manages connections within it's network.
*Figure 6 reprsents the way how Tor network relays data in information circuits. Picture is pretty difficult for layperson.

### Halonen, Ollikainen, Rajala 2023: PhishSticks - The Ethical Hackers tool for BadUSB (Video, about 3 minutes)

* Phishstick is a simulation of maliciously inteded USB memory device that could install e.g keylogger to person's PC if inserted to USB slot of the PC. PhishStick may be very unsusceptile and can contain malware in addition to "needed" information.
* Some people are very unassuming and don't suspect anything at workplace.
* Having employees to freely use any USB memory device on their work PC's can be a security as well as legal risk.
* Companies can protect their employees against malicous USB devices by disabling the feature through e.g. Windows. I have been part of a project that disabled use of non-approved USB memory devices on company devices and while it initially made users very dissatisfied, it was a smart move.

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

Another one is Haystack
![image](https://github.com/user-attachments/assets/50d12531-fbe2-42d8-8d9c-c74a58dff874)

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
![image](https://github.com/user-attachments/assets/9bba32cf-4e87-43af-a608-2bf46d03ddc1)

![image](https://github.com/user-attachments/assets/9d95483e-b908-45a1-a1b5-a9886830bc67)

![image](https://github.com/user-attachments/assets/a6690225-5178-48d6-a8ef-461e0cf04014)


### c) Onion. In your own words, how does anonymity work in TOR? (e.g. how does it use: public keys, encryption, what algorithms? This subtask does not require tests with a computer.)

So, you probably known the movie Shrek. Tor and Shrek (the titular character of the movie) have something in common and that is layers. Like onions. When connecting to Tor network, one's PC connects one computer in Tor network which then connects to next computer in the network and then eventually to the server. Because there are so many connections, server does not relaize it is your computer that is connecting to it, it is some other computer. This is why TOR is very anonymous. Ogres are not that anonymous so in that sense TOR is not like Ogre but kinda is.

![image](https://github.com/user-attachments/assets/99927e5a-9a51-48cf-b86a-52f04076d6bf)

To provide highest level of anonymity, Tor network utilizes many cybe security concepts. All Tor connections are done via Transport Layer Security (TLS) protocol that is used to enable secure connections through internet. There is also encruption in each layer of Tor-Onion to ensure best security levels. Tor uses public keys to ensure high quality authentication. They are called onion keys and are rotated between layers like onions usually are.

I don't quite understand the Onion algorithms so have a picture of fairy godmother on grand piano:

![image](https://github.com/user-attachments/assets/df0910b7-09b4-4d0c-9470-6622df8d71ed)


### d) What kind of the threat models could TOR fit? (This subtask does not require tests with a computer.)

* Using Tor network does not prevent (like we read in article by Karunanayake, Ahmed, Malaney, Islam and Jha 2021: De-anonymisation attacks on tor: A survey.) all threats.
* Internal threats come from company employees: employees can use Tor to bypass all security mechanisms, policies, and controls of the organization and cannot be traced. Employee can share company data anonymously through deep web or sell it to criminals.
* Malware can be injected on exit nodes and that can affect to unencrypted HTTP traffic.
* Use of Tor network can have effect on reputation. If suspcious exit node is part of organisations IP address, the organisation maybe help resposible for crimes made in their IP - without a reason. Examples of these are hacker activity and illegal trade of information/goods. (Ribco)


### e) Don't stick that stick. How does PhishSticks attack work? Would a typical organization be vulnerable? Does this link to a broader category of attacks and defenses? How could the risk be mitigated? (This subtask does not require tests with a computer.) (If you want, you can view PhishSticks on Github and PhishSticks Youtube channel.

*Phishstick works ao that a malicous software (keylogger or something else) is stored in USB memory device and upon inserting USB memory device onto PC, it initializes malware/keylogger that will then distribute e.g. private content such as personal information or password to attacker. Then attacker can properly access to PC through this information. This can be against GDPR or other regulations related organisational (physical) or cyber security.
*Typical organisation would be vulnerable of PhishSticks. Many people are naturally curious and if they find USB memory devices, first reaction is to plug it to USB slot. There is also always a possibility that an intruded accesses to e.g. office space, leaves USB memory device onto someones table with e.g. official looking note and that the person whose desk the USB is on may think that USB device is something they need for work task.
*Thus, typical organisations need to protect themselves with tools like Intune admin templates: https://learn.microsoft.com/en-us/mem/intune/configuration/administrative-templates-restrict-usb that prevent access to USB memory devics unless the employee is authorized to use USB memory devices for theri work. In addition, user training and active communiaction regarding risks that come with USB Devices should not be forgotten about. 


## Sources

Tell me about all the keys Tor uses
https://support.torproject.org/about/key-management/ '

Nethaniel Ribco. 15 November 2023. An Analysis of the Security Risks Posed by Tor Browser
https://www.cyberproof.com/blog/an-analysis-of-the-security-risks-posed-by-tor-browser/

NordVPN
https://nordvpn.com/fi/blog/tor-selain/ 

