# EyeOC

EyeOC is a Google Chrome extension to extract Indicators Of Compromise (IP addresses, emails, hashes) from the active page.

EyeOC will extract:
* IP Addresses
* Domains
* Email Addresses
* Hashes (MD5, SHA256)
* CVEs
* URLs
* Custom Regex

EyeOC will present the user with a JSON blob after processing. The JSON has the following structure:

| Key             | Description                                         |
|-----------------|-----------------------------------------------------|
| url             | URL where extracted data was collected.             |
| time            | Date for the time of collection                     |
| data            | All the data collected, deduplicated and organized. |
| count           | Number of items collected per type.                 |
