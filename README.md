##InformationGathering
Information Gathering Techiques

# To perform information gathering techniques

# AIM:

To perform information gathering techniques using kali linux 

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:
Open terminal/browser and try execute necessary commands/use url to perform information gathering

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified for information gathering:

Footprinting is a part of the reconnaissance process which is used for gathering possible information about a target computer system or network.
http://www.whois.com/whois website to get detailed information about a domain name information including its owner, its registrar, date of registration, expiry, name server, owner's contact information, etc.

## OUTPUT:
<img width="935" height="1033" alt="Screenshot 2026-10-30 072751" src="https://github.com/user-attachments/assets/78485263-a6b1-488e-8622-cf92d8c7b6d2" />



## Finding IP address:
ping command is available on Windows as well as on Linux OS. Following is the example to find out the IP address of chatgpt.com.
```
<img width="786" height="291" alt="image" src="https://github.com/user-attachments/assets/5c0570b4-a5c1-4ea4-bea5-f53d5126baf9" />
```
##output
<img width="846" height="251" alt="image" src="https://github.com/user-attachments/assets/2fb4e103-f2fa-4764-a5aa-b64e2997ca1a" />



## Finding Hosting Company
get further detail by using ip2location.com website.


##output
<img width="751" height="641" alt="Screenshot 2026-10-30 073221" src="https://github.com/user-attachments/assets/68817631-14a6-4b7e-86d0-2e05798b7452" />




## History of the website:
## output
https://web.archive.org/
<img width="962" height="1007" alt="Screenshot 2026-10-30 073826" src="https://github.com/user-attachments/assets/525bf4e1-2921-4872-9144-e3a4cd3fe551" />


# Webserver Fingerprinting:

## Netcat:
```
nc chatgpt.com 80
GET / HTTP/1.1
Host: chatgpt.com
```
#output:
<img width="1920" height="943" alt="image" src="https://github.com/user-attachments/assets/9b9825eb-72ab-4d3b-94b9-3656bf609b0d" />



## nmap:
```
nmap -sL chatgpt.com
```

###output
<img width="805" height="232" alt="image" src="https://github.com/user-attachments/assets/a110b8ec-6b19-4fd4-88f6-467faf8dd9c0" />




## Whatweb:
```
whatweb https://chatgpt.com
```


### output:
<img width="950" height="220" alt="image" src="https://github.com/user-attachments/assets/d94d4e0d-0929-4ae6-b5bf-bcee16bc09b5" />





## httprint
```
httprint -h https://chatgpt.com/ -s /usr/share/httprint/signatures.txt -P0 -t 30000
```
### output:
<img width="560" height="202" alt="terminal_juhijahants_theme" src="https://github.com/user-attachments/assets/a709e1ab-fb38-46a2-b10c-201a77e6c7c8" />








# Tracing the Location
TCP Traceroute:
```
sudo traceroute -T -m 12 -q 1 -w 2 chatgpt.com
```
## output
<img width="736" height="92" alt="image" src="https://github.com/user-attachments/assets/2f999eec-d24c-4cef-adc2-ef997925d9a0" />


## UDP Traceroute:
```
sudo traceroute -U -m 12 -q 1 -w 2 chatgpt.com
```


## output

<img width="673" height="322" alt="image" src="https://github.com/user-attachments/assets/32698761-f2f5-458d-a04e-ef38d9c49dcd" />



## ICMP Traceroute:
```
sudo traceroute -I -m 12 -q 1 -w 2 chatgpt.com
```
## output
<img width="761" height="92" alt="image" src="https://github.com/user-attachments/assets/254a0a87-151b-4c55-9c0a-0807bdd9ef93" />





## RESULT:
The information gathering techniques tools/procedure were  identified successfully
