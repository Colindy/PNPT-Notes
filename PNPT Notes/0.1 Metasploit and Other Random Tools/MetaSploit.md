
`msfconsole`

exploit modules - yea, the actual exploitation of the vulnerability



auxiliary modules - to do things such as port scanning, info gathering, etc.



post modules - post exploitation, after we've compromised the system.




When searching, you can use the search number in the list to load your module or the full path  
&ensp;	`use auxiliary/scanner/smb/smb_version` or `use 388`  
&ensp;&ensp;		Here you are using either the full path or the number in the last search  

Typing `info` once in the module will give you more information about the module.  
&ensp;	There will be fields that will either be required or not.  You'll use `set` to set the field  
&ensp;&ensp;		i.e. `set RHOSTS 10.0.0.3` to set your remote hosts to 10.0.0.3  

Some Post exploitation  
&ensp;	`hashdump` should dump the password hashes from a device that you are connected to in a meterpreter session.  

You can background meterpreter sessions with `background` and then see what sessions you have running with `sessions`.  To join an available session, enter `sessions 1` or whatever number the session you want to join is assigned.  

Setting parameters  
&ensp;	use `set rhosts xxx.xxx.xxx.xxx` to set your options  
&ensp;	use `unset rhosts` to clear out a previously set option  