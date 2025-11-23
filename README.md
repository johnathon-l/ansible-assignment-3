# ansible-assignment-3

Author: Johnathon Laun

## Description

This assignment covers the configuration of two routers using Ansible, with the following requirements:

1. **Configure NTP client on BOTH routers:**  
   - NTP server: `time.google.com` (`216.239.35.0`)

2. **Configure logging on BOTH routers:**  
   - `logging buffered 16384`  
   - `logging console warnings`

3. **Configure DIFFERENT login banners based on router role:**  
   - **router1 (designated as "core"):**  
     Banner = `*** CORE ROUTER - Authorized Access Only ***`
   - **router2 (designated as "distribution"):**  
     Banner = `*** DISTRIBUTION ROUTER - Authorized Access Only ***`

4. **Configure timezone:**  
   - All routers: `clock timezone CST -6`

5. **Verify all configurations**

## How to Run

To execute the script, use the following command:

```sh
ansible-playbook -i inventory.ini assignment3.yaml
```
