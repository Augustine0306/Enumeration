# EXP NO :3
# NAME:AUGUSTINE J
# REGNO:212222240015

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

| Operator    | Description                        | Example Usage           |
| ----------- | ---------------------------------- | ----------------------- |
| `site:`     | Search within a specific domain    | `site:example.com`      |
| `inurl:`    | Search in URL                      | `inurl:admin`           |
| `intitle:`  | Search in page title               | `intitle:"index of"`    |
| `filetype:` | Search by file type                | `filetype:pdf`          |
| `intext:`   | Search inside page text            | `intext:"confidential"` |
| `link:`     | Pages that link to a specific site | `link:example.com`      |
| `cache:`    | View cached version of a site      | `cache:example.com`     |
| `ext:`      | Same as filetype                   | `ext:xls`               |

 ## Architecture 
 ```
+----------------------+
|   Attacker / Hacker  |
|   (Browser & Google) |
+----------+-----------+
           |
           | Google Dork Queries
           v
+---------------------------+
|       Google Search       |
+---------------------------+
           |
           | Indexed Public Content
           v
+---------------------------+
|   Target Websites / Data  |
| - Leaked files            |
| - Open directories        |
| - Sensitive info          |
+---------------------------+

```

# Output:
# SITE:
<img width="956" height="1062" alt="Site exp 3" src="https://github.com/user-attachments/assets/76b2ca96-32b4-42e1-b2b5-68e5879101e9" />

# INURL
<img width="956" height="1067" alt="inurl admin Exp3" src="https://github.com/user-attachments/assets/34f7c706-b367-430f-b29a-43e230499015" />

# INTITLE
<img width="950" height="1065" alt="intitle exp 3" src="https://github.com/user-attachments/assets/3b17d4f6-2685-407e-b54e-a39bd3ed00b1" />

# FILETYPE
<img width="953" height="1057" alt="file type" src="https://github.com/user-attachments/assets/e3ec0026-a26b-4bd8-bc60-7abd9cba2293" />

# INTEXT
<img width="948" height="1060" alt="Intext exp 3" src="https://github.com/user-attachments/assets/cba84167-8aea-4968-a265-744f126322bd" />

# LINK
<img width="952" height="1067" alt="Link exp 3" src="https://github.com/user-attachments/assets/fb5b6ab9-1f63-4f05-933b-992569cee612" />

# CACHE
<img width="952" height="1062" alt="Cache exp 3" src="https://github.com/user-attachments/assets/5f3950f1-01a5-43f9-8744-a0c203909d59" />

# EXT
<img width="948" height="1065" alt="ext exp 3" src="https://github.com/user-attachments/assets/f352a202-b5db-4cbe-9272-545626cf6c6a" />

# DNS Enumeration

<img width="736" height="534" alt="479908719-bf43a1f9-19f3-4a90-a049-14e850f3db49" src="https://github.com/user-attachments/assets/bc8683d9-b894-4a43-aaf1-e4b5bd3f8f3a" />


## DNS Recon

 provides the ability to perform:
 Check all NS records for zone transfers
 Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
 Perform common SRV Record Enumeration
 Top level domain expansion

<img width="746" height="603" alt="479907906-bb21a594-6fae-4950-9a29-98392372574c" src="https://github.com/user-attachments/assets/ca09ee91-6e21-4013-a032-91d87af35d18" />

| Record Type | Meaning                        | Example Output                   |
| ----------- | ------------------------------ | -------------------------------- |
| A           | Host to IPv4 address           | `example.com -> 93.184.216.34`   |
| AAAA        | Host to IPv6 address           | `example.com -> ::1`             |
| MX          | Mail server info               | `mail.example.com`               |
| NS          | Name servers                   | `ns1.example.com`                |
| TXT         | Misc data (SPF, verifications) | `v=spf1 include:_spf.google.com` |
| CNAME       | Canonical names (aliases)      | `www -> example.com`             |

## Common Tools Used (Kali Linux)

| Tool           | Description                                | Usage Example                           |
| -------------- | ------------------------------------------ | --------------------------------------- |
| `nslookup`     | DNS lookup tool (simple queries)           | `nslookup example.com`                  |
| `dig`          | DNS lookup utility (detailed)              | `dig example.com any`                   |
| `host`         | Simple DNS querying tool                   | `host example.com`                      |
| `dnsenum`      | Perl script to enumerate DNS info          | `dnsenum example.com`                   |
| `fierce`       | DNS scanner to locate non-contiguous IPs   | `fierce -dns example.com`               |
| `dnsrecon`     | Powerful DNS enumeration script            | `dnsrecon -d example.com -a`            |
| `theHarvester` | Subdomain enumeration using search engines | `theHarvester -d example.com -b google` |


## OUTPUT:

# NSLOOKUP
<img width="752" height="812" alt="479909190-4d09669d-a5d7-43e9-983a-b87b395dd52f" src="https://github.com/user-attachments/assets/37129fa6-9732-4ad7-9120-09217c3323aa" />

# DIG

<img width="726" height="564" alt="479909853-fec89592-9804-48d2-91a5-5e5636741f9b" src="https://github.com/user-attachments/assets/2195584a-275d-4ae7-a500-f63d4d0a5f25" />

# HOST 

<img width="750" height="447" alt="479909984-67f39315-8ad0-4d37-8536-155e1731829d" src="https://github.com/user-attachments/assets/4cc159fa-cbb6-43d9-b483-e0fd06561256" />

# DNSENUM

<img width="733" height="543" alt="479910262-7c1e5164-50a3-4edc-b3c2-f1d8fb7342f1" src="https://github.com/user-attachments/assets/81b47aae-2231-42e5-a7db-938d0d02ec7f" />

# DNSRECON

<img width="746" height="603" alt="479907906-bb21a594-6fae-4950-9a29-98392372574c" src="https://github.com/user-attachments/assets/e594606e-c21c-4c05-b0d1-706b0c63ceb3" />

# FIERCE

<img width="742" height="762" alt="479912158-3836a9af-37da-448a-ac8d-ae7fbbcee8dd" src="https://github.com/user-attachments/assets/7662a785-2a0c-4ac4-ab89-46e6b3719003" />

# HARVESTOR

<img width="739" height="705" alt="479913848-f31dcc14-9a74-41ee-8ca0-b1bc96359f82" src="https://github.com/user-attachments/assets/c94911ec-fe39-4521-9df1-a84d2984dbe0" />


## Architecture Diagram 
```
+-------------------+        +------------------+       +------------------+
|                   |        |                  |       |                  |
|   Attacker (You)  +------->|   Target Server   +<----->+    DNS Server    |
| Kali Linux / Parrot|       | (Mail / DNS Host) |       |  (Authoritative) |
+---------+---------+        +---------+--------+       +---------+--------+
          |                            ^                          ^
          |                            |                          |
          |                            |                          |
          |           +-----------------------------+            |
          |           |      Information Tools      |            |
          |           |-----------------------------|            |
          |           | smtp-user-enum              |            |
          |           | nmap --script smtp-enum-*   |            |
          |           | dnsenum                     |<-----------+
          |           +-----------------------------+
          |
          v
+-----------------------------+
|   Output/Report             |
|  - Usernames Found          |
|  - MX Records / Zones       |
|  - Subdomains / IPs         |
+-----------------------------+

```

## dnsenum
**Purpose:** A multithreaded Perl script to enumerate information from DNS servers.

**Use case:** Performs DNS zone transfers, brute force subdomains, and gather host IPs.

```
dnsenum example.com
```

## Output:

<img width="736" height="510" alt="479914657-95163872-8224-47b5-adeb-68db81607fb4" src="https://github.com/user-attachments/assets/4810b157-2aee-49de-b157-29a8f5c24610" />


## smtp-user-enum
**Purpose:** Standalone tool used to enumerate valid users by using the VRFY, EXPN, or RCPT TO commands.

**Use case:** Brute-forces SMTP to find users.

```
smtp-user-enum -M VRFY -U users.txt -t <target-ip>
```
  
 ## Output
  
<img width="747" height="415" alt="479915623-df055f43-0a50-48ec-ab9e-9e27218eef4d" src="https://github.com/user-attachments/assets/6c88313e-0b7d-470e-808c-8f1e3cb49187" />


## nmap –script smtp-enum-users.nse <hostname>

**Purpose:** Uses smtp-enum-users NSE script to enumerate valid users on an SMTP server.

**Use case:** Helps identify email accounts on mail servers.

```
nmap -p 25 --script smtp-enum-users.nse <target-ip>
```
## OUTPUT:

<img width="680" height="142" alt="479915907-bf2982f5-e7bb-4537-9a7d-bc5bfed15ad2" src="https://github.com/user-attachments/assets/424de1b0-4fc9-4f79-b1cc-c1dc0bc43deb" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
