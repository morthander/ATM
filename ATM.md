# Setup

Universal | 1HR | 4HR | 1D | 2D | UL | Updated for OWASP.
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Purchase and install a Burp license if you don’t already have one
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Disable the built-in Burp Collaborator functionality
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Install the SwitchySharp Extension in Google Chrome.
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Configure Chrome’s SwitchySharp Extension to point to Burp on localhost:8080 for all protocols.
Universal | 4HR | 1D | 2D | UL | Install the Chrome BuiltWith Extension
Universal | 4HR | 1D | 2D | UL | Configure Burp to save state every 30 minutes to a local directory
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Browse to the site through Chrome and enable auto-forwarding in Burp
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Add your target site(s) to Burp's scope
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Configure Burp to only passively scan in-scope content
Universal | 1D | 2D | UL | Configure Burp to use a 100ms delay between scan requests (with randomness)
Universal | 4HR | 1D | 2D | UL | Install the .NET beautifier Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the Additional Scanner Checks Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the Authz Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the Autorize Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the .NET beautifier Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the Hackvertor Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the Identity Crisis Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the Retire.js Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the Site Map Fetcher Burp Extension
Universal | 4HR | 1D | 2D | UL | Install the SQLiPy Burp Extension

# Familiarity

Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Log in to the application and browse site through Burp for 3-5 minutes; navigate as much functionality as possible
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Watch the Burp proxy traffic for every page you visit
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Note the request format (URL structure)
Universal | 4HR | 1D | 2D | UL | Note the request format (POST structure)
Universal | 4HR | 1D | 2D | UL | Note the cookies being given by the server and sent by the client
Universal | 4HR | 1D | 2D | UL | Note the server platform
Universal | 4HR | 1D | 2D | UL | Note the programming language
Universal | 4HR | 1D | 2D | UL | Note any frameworks in use
Universal | 4HR | 1D | 2D | UL | Document all sensitive functionality
Universal | 4HR | 1D | 2D | UL | List abuse case possibilities for each sensitive function 
Universal | 4HR | 1D | 2D | UL | Brute force domains (where applicable)
Universal | 1HR | 4HR | 1D | 2D | UL | Google for sites site:paypal.com
Universal | 1HR | 4HR | 1D | 2D | UL | Comprehensive nmap scan nmap -sS -A -PN -p- --script=http-title (if in scope)
Universal | 1HR | 4HR | 1D | 2D | UL | Discover platform using danielmiessler.com/services/checkyourstack

# Discovery

Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Find content using RobotsDisallowed (InterestingDirectories.txt)
Universal | 4HR | 1D | 2D | UL | Find content using RobotsDisallowed (Top10000-RobotsDisallowed.txt)
Universal | 1D | 2D | UL | Find content using RobotsDisallowed (Top100000-RobotsDisallowed.txt)
Universal | 1D | 2D | UL | Perform Shodan search of IP range (assuming it's in scope)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Disable form submissions in Burp's Spider settings
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Spider the site using Burp's built-in spidering functionality
Universal | 1HR | 4HR | 1D | 2D | UL | Run Recon-NG's discovery module [ discovery/info_disclosure/interesting_files ]
Universal | 1HR | 4HR | 1D | 2D | UL | Run Recon-NG's Google Site Web module [ recon/domains-hosts/google_site_web ] 

# Automation

Universal | 30M | 1HR | 4HR | 1D | 2D | UL | From the root of the domain in Burp's Target tab, start an Active Scan
Universal | 1HR | 4HR | 1D | 2D | UL | If you have access to another scanner, configure it to the same scope and start it as well
Universal | 4HR | 1D | 2D | UL | If you have access to a third scanner, run it after at least one of the others has finished (be cautious not to cause session drama with manual or other automated testing)
Universal | 1D | 2D | UL | Set Burp’s scanner settings to Thorough and Minimize False Negatives 

# OSINT

Universal | 1HR | 4HR | 1D | 2D | UL | Search Punk spider for your domain to find any existing vulns. [ ReconNG's Punkspider module ]
Universal | 1HR | 4HR | 1D | 2D | UL | Check Google's blacklist for your domain using Nmap. [ nmap --script http-google-malware $target ]
Universal | 1HR | 4HR | 1D | 2D | UL | Check the domain for malware using Nmap [ nmap --script http-malware-host $target ]
Universal | 1D | 2D | UL | Harvest Github repos from company using Recon-NG's github-miner module. [ /recon/companies-multi-github_miner.py ] 
Universal | 1D | 2D | UL | Run Github Dorks against company repos that look interesting [ https://github.com/techgaun/github-dorks ]
Universal | 1D | 2D | UL | Run Gitrob against company repos that look interesting [ https://github.com/michenriksen/gitrob ]
Universal | 1HR | 4HR | 1D | 2D | UL | Run Bluto against the target [ https://github.com/RandomStorm/Bluto ]
Universal | 4HR | 1D | 2D | UL | Run Recon-NG's brute-hosts module on the domain [ recon/domains-hosts/brute_hosts ]
Universal | 4HR | 1D | 2D | UL | Run Recon-NG's [ recon/domains-hosts/brute_hosts ] 

# Authentication

Universal | 30M | 1HR | 4HR | 1D | 2D | UL | User enumeration due to response differentiation; check timing differences between failed auth on real user vs. non-existent user
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Password reset mechanism (cleartext password sent)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Password reset mechanism (guessable token)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Password reset mechanism (reusable token)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Password reset mechanism (reuse of token doesn’t generate an alert)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Password reset mechanism (token doesn’t expire)
Universal | 1HR | 4HR | 1D | 2D | UL | Password reset mechanism (reusable token)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | User enum via message on password reset
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | User enum via message on login
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | User enum via message on registration
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Lack of account lockout
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Password not required to perform sensitive account actions (email change)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Password not required to perform sensitive account actions (password change)
Universal | 4HR | 1D | 2D | UL | Password not required to perform sensitive account actions (shipping address change)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Password not required to perform sensitive account actions (mailing address change)
Universal | 4HR | 1D | 2D | UL | Email address can be changed for arbitrary users without authorization
Universal | 4HR | 1D | 2D | UL | Shipping address can be changed for arbitrary users without authorization
Universal | 1HR | 4HR | 1D | 2D | UL | Sensitive data can be changed within an account without asking for the user’s password

# Session Management

Universal | 1HR | 4HR | 1D | 2D | UL | Cookies not invalidated after logout
Universal | 1HR | 4HR | 1D | 2D | UL | New cookie not given upon login
Universal | 1HR | 4HR | 1D | 2D | UL | Reversible cookies (base64, etc.)
Universal | 1HR | 4HR | 1D | 2D | UL | Multiple sessions allowed
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Multiple sessions allowed without notification
Universal | 4HR | 1D | 2D | UL | Sensitive functions do not contain CSRF defenses
Universal | 4HR | 1D | 2D | UL | Determine if access to sensitive resources is being granted due to referer header
Universal | 4HR | 1D | 2D | UL | Use Burp’s Identity Crisis to determine if URLs respond differently based on User Agent strings
Universal | 1HR | 4HR | 1D | 2D | UL | Sensitive pages or actions within one context can be forcefully browsed or executed to by other/lower users, e.g. viewing a profile, viewing a report, viewing messages, etc.
Universal | 4HR | 1D | 2D | UL | Make a list of all sensitive functions on the site, execute each one thoroughly, and analyze all proxy traffic during each of their workflows
Universal | 4HR | 1D | 2D | UL | Explore all numeric values that appear to be identifiers, e.g., UIDs, GUIDs, etc. Rotate those values both within the URL and in POST parameters and see if you can access other contexts
Universal | 4HR | 1D | 2D | UL | Attempt to fall back to HTTP for sensitive functions

# Input Validation

Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Set Burp’s scanner settings to enable URL to Body and Body to URL
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Perform a Burp active scan against the root of the site. If you receive authentication failures, lower your number of threads and/or increase the delay between requests
Universal | 1HR | 4HR | 1D | 2D | UL | Intruder on key fields using SecLists XSS (look for field markers)
Universal | 1HR | 4HR | 1D | 2D | UL | Intruder on key fields using SecLists SQLi (look for field markers)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Intruder on key fields using SecLists Polyglots (look for field markers)
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | For any SQLi discovered, exploit using standalone SQL Map instance
Universal | 4HR | 1D | 2D | UL | Test the target with XSS polyglots [ https://github.com/danielmiessler/SecLists/blob/master/Fuzzing/Polyglots/XSS_Polyglots.txt ] 
Universal | 4HR | 1D | 2D | UL | Test the target with SQLi polyglots [ https://github.com/danielmiessler/SecLists/blob/master/Fuzzing/Polyglots/SQLi_Polyglots.txt ] 
Universal | 4HR | 1D | 2D | UL | Test for RFI manually.
Universal | 4HR | 1D | 2D | UL | Test for LFI manually.

# Logic Testing

Universal | 1HR | 4HR | 1D | 2D | UL | Test CAPTCHAs for replay attacks
Universal | 1HR | 4HR | 1D | 2D | UL | Test CAPTCHAs for cleartext disclosure in source
Universal | 1HR | 4HR | 1D | 2D | UL | Test CAPTCHAs for removal of CAPTCHA field in request
Universal | 1HR | 4HR | 1D | 2D | UL | Test 2FA for removal of 2FA field in request
Universal | 1HR | 4HR | 1D | 2D | UL | Test 2FA for skip ahead attack
Universal | 1HR | 4HR | 1D | 2D | UL | Test e-Commerce sites for skip ahead attacks (skip payment and move to shipping)
Universal | 1HR | 4HR | 1D | 2D | UL | Test e-Commerce sites for handling of negative numbers
Universal | 4HR | 1D | 2D | UL | Test sensitive functions for addition of repeated parameters that have different values

# Platform Testing

Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Full portscan of the system (assuming scope) [ nmap -sUS -p- -A -oA target $target ]
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Within the proxy traffic, look for any signs of HTTP fallback
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Check the server headers for security-oriented ones [ X-Frame-Options, Strict-Transport-Security, X-XSS-Protection, Content-Security-Policy, X-Content-Security-Policy,  etc. ] [ http://cyh.herokuapp.com/cyh ]
Universal | 30M | 1HR | 4HR | 1D | 2D | UL | Scan for use of insecure HTTP methods
Nginx | 1HR | 4HR | 1D | 2D | UL | Nginx was detected: check Nginx vesion and look for vulnerabilities
Express | 4HR | 1D | 2D | UL | Express was detected. Check for versions and any associated issues
Node | 4HR | 1D | 2D | UL | Node was detected. Check for versions and any associated issues
Apache | 4HR | 1D | 2D | UL | Apache was detected: check Apache version and look for vulnerabilities
Wordpress | 30M | 1HR | 4HR | 1D | 2D | UL | Scan the site with CMSMap
SAP | 4HR | 1D | 2D | UL | Check all sensitive transaction codes.