# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

## OUTPUT
site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
<img width="1234" height="1027" alt="Screenshot 2025-11-09 172247" src="https://github.com/user-attachments/assets/c15a3818-ebbd-4d9d-b36d-f28baacb9401" />
## OUTPUT
filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
<img width="1238" height="1023" alt="Screenshot 2025-11-09 172643" src="https://github.com/user-attachments/assets/dcbce642-44d7-42ef-a293-183d979df89e" />
## OUTPUT
intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
<img width="1230" height="1013" alt="Screenshot 2025-11-09 172544" src="https://github.com/user-attachments/assets/8a6a778c-ddbf-465a-9254-cbc30d8b2ca1" />

## OUTPUT
inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="1239" height="1033" alt="Screenshot 2025-11-09 172416" src="https://github.com/user-attachments/assets/bb116293-d240-4564-9ad1-0638f219f0d3" />
## OUTPUT
intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
<img width="1237" height="1021" alt="Screenshot 2025-11-09 172209" src="https://github.com/user-attachments/assets/c83fbc12-a48a-4cbe-8ac2-ee8f135b8e9b" />

## OUTPUT
link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="1227" height="1017" alt="Screenshot 2025-11-09 172303" src="https://github.com/user-attachments/assets/95db5554-73ca-4043-ae56-9202573ebcd7" />

## OUTPUT
cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
<img width="1234" height="1024" alt="Screenshot 2025-11-09 173157" src="https://github.com/user-attachments/assets/c61c9041-42be-42aa-bd17-fb801e3b14ca" />

 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

<img width="765" height="615" alt="Screenshot 2025-11-17 092039" src="https://github.com/user-attachments/assets/3f1f2730-f566-4582-b9a8-4b16e38e104e" />

##dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## OUTPUT
<img width="638" height="460" alt="Screenshot 2025-11-17 090543" src="https://github.com/user-attachments/assets/04ea280b-bd2e-4302-94f1-61844fb5c81d" />

##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
  
## Output

  <img width="628" height="432" alt="Screenshot 2025-11-17 092120" src="https://github.com/user-attachments/assets/8336f702-e418-404d-8f0d-4e10dd5ab6e6" />

In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
<img width="1389" height="885" alt="Screenshot 2025-10-20 123210" src="https://github.com/user-attachments/assets/c21c1b6c-16ce-4e07-9031-1d22fc450202" />

select any username in the first column of the above file and check the same


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
  <img width="563" height="280" alt="Screenshot 2025-11-17 092900" src="https://github.com/user-attachments/assets/5d9d3ca4-95bf-4c30-ad11-9d7791662f01" />

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="616" height="185" alt="Screenshot 2025-11-17 093131" src="https://github.com/user-attachments/assets/dfa6c384-fbaf-443f-b10c-722a464735ab" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

