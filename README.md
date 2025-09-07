# HTSECURE
A custom hardened .htaccess implementattion for LAMP Stack users

## Current functionality:
- Protection againt dozens of attack vectors
- Protection against bypass methods for these attack vectors
- Removal of ServerSignature and other info that could potentially be sensitive
- Removal of all file extensions from URL's
- Blacklisting of many common names for publicly-used webshells
- IP-Based whitelisting for access to admin panel
- Logging of all malicious activity
- All open directories autokmatically set to give HTTP 403 response
- Custom error message outputs for 401/403/404 errors
- Prevention of file execution within uploads directories
- Prevention of file execution within directories to store temporary files
- Various performance optimization methods implemented
- Block suspsicious user agents
- Block traffic coming from many well-known web-based exploitation tools
- Application-specific protections (Wordpress, Joomla, Drupal, etc)
- Prevention of reading potentially-sensitive files (.env, .DS_STORE, etc)
- Automatically sets various HTTP security-related rseponse headers (CSP, X-frame-options, referrer-policy, x-download-options, etc)
- Automatically unsets/disables HTTP headers whhich could reveal info about the systen (server, ETag, X-powered-by, etc)

## TO-DO:
- Add protections for additional attack vectors
- Add automatic setting of a larger number of security-related HTTP response headers
- Implement more comprehensive logging
- Add wayyyyyy more restrictions on potential filter bypass methods for potential attack vectors
- Implement a larger number of CMS-Specific protections
- Implement more performance optimization techniques
