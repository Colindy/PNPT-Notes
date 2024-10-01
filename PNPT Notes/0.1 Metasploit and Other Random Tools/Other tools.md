### A couple other tools  

`dnsrecon -r 127.0.0.0/24 -n 10.0.2.154 -d blah`  
&ensp;	dnsrecon will scan the devices dns (if 53 is open) and return records  
&ensp;	-r is for range on the device to check  
&ensp;	-r is the ip of the target  
&ensp;	-d is for the domain (isn't always relevant but dnsrecon will not run without it)  
&ensp;&ensp;			`python3 -m pip install -U pyOpenSSL cryptography`  
&ensp;&ensp;			If you get `python OpenSSL_add_all_algorithms` error  
&ensp;&ensp;			This happens when there is an incompatibility between cryptography and pyOpenSSL  

`hashcat -m 0 hashes.txt /usr/share/wordlists/rockyou.txt`  
&ensp;	-m 0 is the hash type.  you can use `hashcat --help | grep <hash type>` to search for this code  
&ensp;	hashes.txt is the file you have the hash stored in  
&ensp;	/usr/......./rockyou.txt is the file to check against for comparison  
&ensp;&ensp;		This tool should always be run using the GPU for maximum effect, never in a VM if it can be avoided.  
&ensp;	-O   Will optimize the process of running hashcat  
&ensp;	-r   Will run rule sets against the list as well.  One Rule to Rule them All is a popular one  