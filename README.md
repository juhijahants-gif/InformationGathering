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
<img width="786" height="291" alt="image" src="https://github.com/user-attachments/assets/1977eab9-02a1-4f54-9ea7-c7f358bc17de" />



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
<img width="1920" height="943" alt="image" src="https://github.com/user-attachments/assets/9c735c32-a7eb-4c5b-913e-a2d51c311da8" />




## nmap:
```
nmap -sL chatgpt.com
```

###output
<img width="797" height="192" alt="image" src="https://github.com/user-attachments/assets/52c74e38-bc18-4189-b312-4a35ae9477b5" />



## Whatweb:
```
whatweb https://chatgpt.com
```

### output:
<img width="985" height="255" alt="image" src="https://github.com/user-attachments/assets/32de84a8-5170-47c4-bdab-c2926dc2bfd7" />



## httprint
```
httprint -h https://chatgpt.com/ -s /usr/share/httprint/signatures.txt -P0 -t 30000
```
### output
<img width="2170" height="725" alt="image" src="https://github.com/user-attachments/assets/fd0b7980-590a-43d0-bbd2-7f089862f615" />




# Tracing the Location
TCP Traceroute:
```
sudo traceroute -T -m 12 -q 1 -w 2 chatgpt.com
```
## output
<img width="787" height="137" alt="image" src="https://github.com/user-attachments/assets/57d33d7d-25e1-467f-8c1b-2f25aad24e3e" />


## UDP Traceroute:
```
sudo traceroute -U -m 12 -q 1 -w 2 chatgpt.com
```


## output

<img width="735" height="367" alt="image" src="https://github.com/user-attachments/assets/d8e5f7e0-2b4b-4041-9459-9b9169971450" />


## ICMP Traceroute:
```
sudo traceroute -I -m 12 -q 1 -w 2 chatgpt.com
```
## output
<img width="757" height="125" alt="image" src="https://github.com/user-attachments/assets/043d8d4e-533b-42d7-b983-ce0a2535ae46" />




## RESULT:
The information gathering techniques tools/procedure were  identified successfully
