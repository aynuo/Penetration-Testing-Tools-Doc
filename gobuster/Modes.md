# Gobuster mods

## Directory mode
* Scans for directories on a web server.

`gobuster dir -u <target_url> -w <wordlist_file>`

## DNS mode
* Enumerates subdomains using DNS queries.

`gobuster dns -d <domain> -w <wordlist>`

## Vhost mode
* Tests for virtual hosts on a web server.

`gobuster vhost -u <URL> -w <wordlist> -t <threads>`

## IP mode
* Scans for active IP addresses within a specified range.

`gobuster ip -r 192.168.1.0/24 -n networks.txt -t 5`

## CNAME mode
* Identifies canonical names associated with a domain.

`gobuster cname -d <domain> -w <wordlist>`

## S3 mode
* Searches for S3 buckets in Amazon Web Services.

`gobuster s3 -u <URL> -w <wordlist>`

## Endpoint mode
* Explores REST API endpoints for a given target.

`gobuster endpoint -u <URL> -w <wordlist>`

## HTTP methods mode
* Tests different HTTP methods (GET, POST, PUT, DELETE, etc.) on a web server.

`gobuster http-methods -u <URL> -w <wordlist> -x <extensions> -t <threads>`

## TLS mode
* Checks for SSL/TLS certificate information.

`gobuster tls -u <URL> -w <wordlist> -k <insecure> -t <threads>`

## File mode
* Searches for specific files or file extensions on a web server.

`gobuster file -u <URL> -w <wordlist> -x <extensions> -t <threads>`

## FUZZ
allows for automated testing by iterating through a wordlist and replacing a specific part of the URL.

`gobuster file -u <URL> -w <wordlist> -x <extensions> -t <threads>`