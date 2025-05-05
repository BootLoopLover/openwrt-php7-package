
Compile PHP7 modules
====================

Follow the cross compile tutorial on the Omega site
https://wiki.onion.io/Tutorials/Cross-Compile

In the step 3, add the PHP7 repo

```
echo "src-git php7 https://github.com/BootLoopLover/openwrt-php7-package.git" >> feeds.conf.default
```

```
scripts/feeds update -a
scripts/feeds install -a
```


#make menuconfig 
Language/php/php7
tick 
```
<*> php7......................................... PHP7 Hypertext preprocessor               
[*] PHP7 LIBXML support                                                                     
[*] Use system timezone data instead of php's built-in database                    
-*- php7-cgi..................... PHP7 Hypertext preprocessor (CGI & FastCGI)                  
<*> php7-cli............................... PHP7 Hypertext preprocessor (CLI)                   
<*> php7-fastcgi...................................... FastCGI startup script                    
<*> php7-mod-curl......................................... cURL shared module                    
<*> php7-mod-fileinfo................................. Fileinfo shared module
```       
 
