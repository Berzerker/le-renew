# LetsEncrypt Renewal Script

Renewal Script for LetsEncrypt certs

# Notes
- Default authenticator method stops web server to temporarily bind 443 to test DNS on requested domains
- Edit .ini file to add email and comma-separated domains
- NOT for initial pull, run a certbot command separately first, then set this to renew

# Installation
- le-renew is the bash script to renew, edit variable to point to .ini config file
- Edit le-renew.ini with required information
- For added security, permission down to only required for both files read/execute access
- Cron le-renew to run once every couple days, will update once script reaches 10 days until expiration.
