# Nmap Cheat Sheet
## Basic Usage

1. **Scan a Single Host:** `nmap <target>`
2. **Scan Multiple Hosts:** `nmap <target1> <target2>`
3. **Scan an Entire Subnet:** `nmap <target>/24`

## Scan Techniques

1. **TCP SYN Scan:** `nmap -sS <target>`
2. **TCP Connect Scan:** `nmap -sT <target>`
3. **UDP Scan:** `nmap -sU <target>`
4. **TCP ACK Scan:** `nmap -sA <target>`
5. **OS Detection:** `nmap -O <target>`
6. **Service Version Detection:** `nmap -sV <target>`

## Output Options

1. **Save Results to a File:** `nmap -oN output.txt <target>`
2. **Verbose Output:** `nmap -v <target>`
3. **Aggressive Scan:** `nmap -A <target>`
4. **Save Output in XML Format:** `nmap -oX output.xml <target>`
5. **Save Output in All Formats:** `nmap -oA output <target>`

## Timing Options

1. **Paranoid Timing:** `nmap -T0 <target>`
2. **Sneaky Timing:** `nmap -T1 <target>`
3. **Polite Timing:** `nmap -T2 <target>`
4. **Normal Timing:** `nmap -T3 <target>`
5. **Aggressive Timing:** `nmap -T4 <target>`
6. **Insane Timing:** `nmap -T5 <target>`

## Other Useful Options

1. **Ping Scan:** `nmap -sn <target>`
2. **Skip DNS Resolution:** `nmap -n <target>`
3. **Exclude Hosts:** `nmap --exclude <excluded_target> <target>`
4. **Show Open Ports Only:** `nmap --open <target>`
5. **Fast Scan:** `nmap -F <target>`
6. **Verbose Output without DNS Resolution:** `nmap -nv <target>`