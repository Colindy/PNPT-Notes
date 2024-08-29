`dnsrecon -r 127.0.0.0/24 -n 10.0.2.154 -d blah`
	dnsrecon will scan the devices dns (if 53 is open) and return records
	-r is for range on the device to check
	-r is the ip of the target
	-d is for the domain (isn't always relevant but dnsrecon will not run without it)
			`python3 -m pip install -U pyOpenSSL cryptography`
			If you get `python OpenSSL_add_all_algorithms` error
			This happens when there is an incompatibility between cryptography and pyOpenSSL

`hashcat -m 0 hashes.txt /usr/share/wordlists/rockyou.txt`
	-m 0 is the hash type.  you can use `hashcat --help | grep <hash type>` to search for this code
	hashes.txt is the file you have the hash stored in
	/usr/......./rockyou.txt is the file to check against for comparison
		This tool should always be run using the GPU for maximum effect, never in a VM if it can be avoided.
	-O   Will optimize the process of running hashcat
	-r   Will run rule sets against the list as well.  One Rule to Rule them All is a popular one