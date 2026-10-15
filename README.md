# Ancora-Education-Ucertify-Lab23
# Scanning Systems in Ubuntu Linux

> **Original Lab Source**
> 
> This lab was available through:
>
> [https://ancoraeducation.ucertify.com/app/?func=navigate_items&item_sequence=6]

## Instructions
In this lab, you'll learn to scan systems in Ubuntu Linux using the Netcat utility. Netcat is a simple utility that reads and writes data across network connections using TCP or UDP protocols. Netcat is included with several distributions of Linux, including Debian (of which Ubuntu is a variant). 

To scan systems in Ubuntu Linux using the Netcat utility, here's what you need to do:

1.On the desktop, click to open the Terminal window and then execute the following command:
```bash
echo QUIT | nc -v -v -z -w 3 127.0.0.1 20-81
```

**NOTE**

This command instructs Netcat to enter verbose mode (-v -v) to receive more output. It scans Ports 20 through 81, inclusive. The -z option tells Netcat not to bind a port to the local address, so you need not press enter to escape the service. The -w 3 option tells Netcat to wait a maximum of three seconds at a port, in case one somehow binds in spite of the -z option.

2.You now have scanned your host to view some of the open ports. 

Note: While scanning the host, the output may vary based on the concept that which ports are open and which ports are not open.

3.Notice that this scanner does not report any vulnerabilities. However, it is useful because when used as a scanner, it works quickly.

## Disclaimer

This repository is for **educational and personal learning purposes only**.  

The original lab content belongs to **uCertify / Ancora Education** and remains their copyrighted material.  
This repository is not affiliated with, endorsed by, or sponsored by uCertify or Ancora Education.  

No copyright infringement is intended.  
Use of any tools or techniques mentioned here should only be performed in authorized, legal environments.
