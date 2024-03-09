# DNSenum

## Description
DNSenum is a versatile tool used for information gathering in the domain name system (DNS) infrastructure. It facilitates the enumeration of DNS records to gather valuable information about a target domain, such as hostnames, subdomains, mail servers, and more. DNSenum is an essential tool in penetration testing, network security assessments, and bug bounty hunting.

## Installation
DNSenum can be installed on various Linux distributions using package managers or from the source code available on GitHub. Follow the steps below for installation:

1. **Using Package Manager:**

   ```
   sudo apt-get install dnsenum
   ```

2. **From Source:**
   - Clone the repository from GitHub:

     ```
     git clone https://github.com/fwaeytens/dnsenum.git
     ```
   - Change directory to the dnsenum folder:

     ```
     cd dnsenum
     ```
   - Install the dependencies:

     ```
     sudo apt-get install libnet-perl libnet-dns-perl libnetaddr-ip-perl
     ```
   - Run the installer:

     ```
     perl Makefile.PL
     make
     sudo make install
     ```

## Usage
DNSenum offers various options for DNS enumeration. Below are some common usage examples:

- Enumerate DNS records for a specific domain:

  ```
  dnsenum example.com
  ```

- Perform zone transfer:

  ```
  dnsenum --enum -f dns_servers.txt example.com
  ```

- Enumerate DNS records with additional information:

  ```
  dnsenum --enum -v -f dns_servers.txt example.com
  ```

## Options
- **--enum**: Perform DNS enumeration.
- **-f**: Specify a file containing DNS servers.
- **-v**: Enable verbose mode to display detailed output.

## Examples
1. Enumerate DNS records for example.com:

   ```
   dnsenum example.com
   ```

2. Perform zone transfer for example.com using specified DNS servers:

   ```
   dnsenum --enum -f dns_servers.txt example.com
   ```

3. Enumerate DNS records with additional information:

   ```
   dnsenum --enum -v -f dns_servers.txt example.com
   ```

## References
- GitHub Repository: [https://github.com/fwaeytens/dnsenum](https://github.com/fwaeytens/dnsenum)
- DNSenum Documentation: [https://github.com/fwaeytens/dnsenum/wiki](https://github.com/fwaeytens/dnsenum/wiki)
