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

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain  tourism.ap.gov.in 

<img width="1886" height="870" alt="image" src="https://github.com/user-attachments/assets/39b94e3d-9d59-49d7-bf09-2f6577131743" />

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain  tourism.ap.gov.in 

<img width="1919" height="878" alt="image" src="https://github.com/user-attachments/assets/18062c18-5c75-4509-9b04-7da8387df8e2" />

intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

<img width="1904" height="868" alt="image" src="https://github.com/user-attachments/assets/6229a664-9cd6-48a7-afed-1cfe22b9e0ad" />


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="1916" height="865" alt="image" src="https://github.com/user-attachments/assets/e0830d0f-655a-497d-85b4-fce402e63b1a" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
<img width="1918" height="872" alt="image" src="https://github.com/user-attachments/assets/d4c3d35f-4919-4a55-a0cb-180e2879eef7" />

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="1648" height="876" alt="image" src="https://github.com/user-attachments/assets/7c5edd87-a735-4f8d-ae25-219c08d03b31" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

<img width="1802" height="692" alt="image" src="https://github.com/user-attachments/assets/f3752905-7aa2-4316-bdb9-8b9244cbacdb" />
 
# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
<img width="955" height="185" alt="image" src="https://github.com/user-attachments/assets/8495a58b-7a85-4a53-a09e-5c7170154cdc" />


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

<img width="944" height="283" alt="image" src="https://github.com/user-attachments/assets/3cd3cb95-15f9-42b3-9678-a63f75443e10" />


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
<img width="954" height="338" alt="image" src="https://github.com/user-attachments/assets/f98029a0-6a04-4249-8339-84f9b79b1dcc" />


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

<img width="716" height="397" alt="image" src="https://github.com/user-attachments/assets/21026773-c7f2-4656-a48e-0334f940cf21" />



# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
<img width="1249" height="457" alt="image" src="https://github.com/user-attachments/assets/d1c0ce12-da3b-4021-a870-16dcae90f732" />
  

## nmap –script smtp-enum-users.nse <hostname>
 
The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="936" height="167" alt="image" src="https://github.com/user-attachments/assets/dc662551-0942-4e0b-9577-c3426ce528ac" />



## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

