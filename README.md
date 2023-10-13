### DOMAIN NAME SERVICE
Name Cheap
```
Setup Email Server

1. Select the Domain name to setup
2. Chooose DNS Manager/ Host Record
3. Choose NameCheap basic DNS
4. Select update Host Record
5. Edit your Host Record
```
```
Note:
- DNS Manager/ Host Record will be enabled if you use NameCheap defautl DNS Servers
- You can setup Multiple Name Server in different Host Record (NameCheap and Interserver(VPS))
```
### Setup Business Email
Zoho
```
Setup Business Email

1. Sign-in via Google Account
2. Verity domain name by adding the TXT Record in DNS Manager/ Host Record
3. You may check the A, TXT, MX, NS in Zoho lookup
4. Add additional TXT Records in DNS Manager/ Host Record
5. Create your Business email johnmarkroco@iwebitechnology.xyz
```
```
Note:
- Verification of Zoho can only be used in your Domain Name DNS Provider (NameCheap)
  not The thirdparty (Interserver)
```
### Important Terminologies on DNS
```
A Record  - Domain name pointing to VPS Public IP Address
TXT       - Plain Text used for Host verification/ Short Message
MX Record - Mail Exchange direct email to mail server i.e. (mx.zoho.com.)
CNAME     - Domain name pointing to other Domain name
```
### Troubleshooting
Flush DNS Ubuntu
```
$sudo systemd-resolve --flush-caches
$sudo systemd-resolve --statistics 
```
Unable Verify Zoho Account (Using a Third Party Hosting Provider ) (NameCheapt and Interserver)
```
Trick: 
1. In NameCheap use NameCheap Default  Name Server to enable Host Record.
2. You need to verify it through your Domain Provider Host Record (in my case NameCheap)
   a. Add the TXT records and MX records
3. After the verifications (you proved you own the Domain Name)
4. You can now copy the TXT and MX records to your third party (Hosting Provider)
5. Setup again the NameCheap to use your Third Party Name Server of Interserver
```
