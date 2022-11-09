# Honeypot Assignment

**Time spent:** **4** hours spent in total

**Objective:** Create a honeynet using MHN-Admin. Present your findings as if you were requested to give a brief report of the current state of Internet security. Assume that your audience is a current employer who is questioning why the company should allocate anymore resources to the IT security team.

### MHN-Admin Deployment (Required)

**Summary:** The deployment went quite easily. I just followed the written instructions adn deployed the mhn-admin through google cloud.

![MHN-admin Proof](https://user-images.githubusercontent.com/60580593/200932546-b225c8a0-f73d-4936-aa36-8f0adf872830.gif)

### Dionaea Honeypot Deployment (Required)

**Summary:** The Dionaea script initalizes the machine as a honeypot  and connects it to the mhn-admin console. 

![Honeypot proof](https://user-images.githubusercontent.com/60580593/200930105-9e6d2a5f-c93c-49e0-bd47-6f8ee3382b96.gif)

### Database Backup (Required) 

**Summary:** The RDBMS is a SQL database. The json is the file that includes all of the information of attackers scanning and trying to connect to the honeypot. 

*Be sure to upload session.json directly to this GitHub repo/branch in order to get full credit.*

### Deploying Additional Honeypot(s) (Optional)

#### 2 Honeypot

**Summary:** This honeypot is used to monitor traffic coming in from all across the world and can be used to monitor new malware coming in. 

![Honeypot proof](https://user-images.githubusercontent.com/60580593/200928295-55373968-ad39-49e2-8261-1eeb93f56cd6.gif)


### Malware Capture and Identification (Optional)

#### 1 Malware

**Summary:**I found it through the mhn-admin payload section which gives the hashes of the payloads that come in. This was the first one I searched on virustotal and it came up as a trojan which attacks CVE-2017-0147. 

MD5 Hash: 9cc600b0c21a0ee60257aa9d5aaf0b44

SHA1 Hash: db1235d751265b755f61112cb826732307ade2faeabcb6892483e17c8c716719fa41e546072eeab993b6e672dcde686f2ecb9e63acbcc7911e10fe706fcec02e	

![Malware Capture](https://user-images.githubusercontent.com/60580593/200928269-c40b7dd7-3126-4130-9691-0ace4f1a1e68.gif)

## Notes: The only issue I had was in trying to connect to mhn-admin after deploying it. I was connecting via port 3000 because I saw that as a port listed in the command line. That port only shows the map and has no UI. I had to do some looking around to realize I needed to use port 80. It should have been obvious but it took me about 15 minutes.

Describe any challenges encountered while doing the assignment.
