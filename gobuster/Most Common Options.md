# Most Common Options

## -u
* This option specifies the target URL to be scanned by Gobuster. It tells Gobuster where to start its directory and file brute-forcing.

`gobuster dir -u https://example.com`

## -w  <wordlist directory>
* allows you to specify the path to a file containing a list of potential directory and file names to be used in the brute-force attack. This is a crucial parameter as it determines the scope of the scan.

`gobuster dir -u https://example.com -w /usr/example.txt` 

## -x
* you can specify a list of file extensions to be appended to each directory name in the wordlist. Gobuster will then attempt to identify files with these extensions in the discovered directories.

`gobuster dir -u https://example.com -w /usr/example.txt -x png`

## -t
* allows you to set the number of concurrent threads to be used in the brute-force scan. Increasing the number of threads can speed up the scan but may also increase server load and network traffic.
* Default Threat is 10 

`gobuster dir -u https://example.com -w /usr/example.txt -t 100`

## -s
* allows you to specify the HTTP status codes to be treated as valid responses.
* By default, Gobuster considers only status codes in the 200 range as valid. 

`gobuster dir -u https://example.com -w /usr/example.txt  --status-codes-blacklist "" -s 200,301,401`

## -r
* The recursive option enables recursive directory brute-forcing, allowing Gobuster to explore directories within directories.

`gobuster dir -u https://example.com -w /usr/example.txt -r`

## -c
* specify HTTP cookies to be included in requests sent by Gobuster.

`gobuster dir -u https://example.com -w /usr/example.txt -c "your cookies"`

## -k
* This option instructs Gobuster to ignore SSL certificate validation errors.

`gobuster dir -u https://example.com -w /usr/example.txt -k`

## -q
* only displays the results of the scan.

`gobuster dir -u https://example.com -w /usr/example.txt -q`











