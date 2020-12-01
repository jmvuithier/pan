# Palo Alto Network Best Practice

### Change to "set" mode on the firewall with cli

The goal of this repository is to improve the basic configuration of Palo Alto Networks Firewall

Run the following command to view the configuration:

"set" format:
> set cli config-output-format set

> configure
> show 

### How to use the set files

1. Download the source on your computer
2. Edit the file in your favorite editor (like bbedit, notepad++ etc...)
3. Connect on ssh on your firewall 
4. type "set cli config-output-format set
5. Pass on "configure"
6. Past the file like wildfire.set
7. "commit" 
8. Connect on the gui and check the result 

### Wilfire configuration

The file "wilfire.set" contain the basic configuration

### Define basic objects

the file "objects.set" contain the minimal objects (Sinkhole Google DNS etc...)

### Define scheduled

the file "scheduled.set" contain the scheduled time for "update"


### Define mail relay (for report and alert)

the file "mailconfig.set" contain the mail configuration


### Define Sinkhole rule

the file "Rule_DNS_Sinkhole_Block.set" contain Block Sinkhole_Block packet from Any to Any


### Define No-Decrypt rule

the file "No-Decrypt-Rule.set" contain a best practice for no decrpyt standard categories and "WhiteList and BlackList" 

### Decryption_Profile

the file "Decryption_Profile.set" contain a best practice for Decryption 

### Threat-Prevention

the file "Threat-Prevention.set" contain a best practice for Antivirus, AntiSpyware, Url Filtering, Wildfire, FileBlocking on this
configuration multiple profile and groups are created for Inbound and Outbound traffic
