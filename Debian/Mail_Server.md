
# By T3d 
I' am :manfirefighter:
## MAIL SERVER: POSTFIX

## INSTALLATION

For mail server installation you should install __postfix__ (mail server) </br> 
and __sasl2-bin__(database adminstration for mail server(i think , (i re-precise (i think)))) </br>
</br>
##CLI INSTALL 
:fire:
` sudo apt install postfix sasl2-bin` </br>


### Error 
1. Sasl2-bin :Jack-O-Lantern:
_Postfix_ installation slide but we seen one error because `sasl2-bin` depend of `db-util` </br>

_Error_: sasl2-bin: Depend: db-util is not install (or others sentense like this) </br>
 2. 
When you try to install db-util with `sudo apt install sasl2-bin` you observe others error </br> 
## Resolve Bugs and Error</br>

Go to `pkgs.org`[pkgs.org for amd64 system](https://debian.pkgs.org/10/debian-main-amd64)  where i take this link [sasl2-bin](https://debian.pkgs.org/10/debian-main-amd64/sasl2-bin_2.1.27+dfsg-1+deb10u2_amd64.deb.html)  </br> 


 
To install `bd-util`  </br> 


## db-util install

	`wget http://ftp.de.debian/pool/main/d/db-defaults/db-defaults/db-util_5.3.1+nmu1_all.deb`    
	
		`sudo dpkg -i db-util_5.3.8+nmu1_all.deb`
 </br>
## 3th error 

 db-util depend on db5.3-util and this package is not install  </br>

## Resolve 3 error  </br>
:key:
	`wget http://ftp.de.debian/pool/main/d/db-5.3/db5.3-util_5.3.28+dfsg1-0.5_amd64`  </br>
	
	sudo dpkg -i db5.3-util_5.3.28+dfsg1-0-5_amd64.deb  </br>
 </br>
and re-try  </br>

	`sudo dpkg -i db-util_5.3.8+nmu1_all.deb` 

and 
	
	`sudo apt install postfix sasl2-bin`  </br>

	 Choice 'No configuration' when the special shell interface display
	 
	 
	😹️`Bug out`


# Next 

## Server-world

[server-world](https://www.server-world.info/en/note?os=Debian_10&p=mail&f=1)

End
