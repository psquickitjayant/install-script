File Monitoring Script
======================

Configure your any text file to send it contents to Loggly

    chmod 755 configure-file-monitoring.sh
    sudo ./configure-file-monitoring.sh -a SUBDOMAIN -u USERNAME -f FILENAME -l FILE_ALIAS
    
**Notes:**
<ol>
 <li>File Alias should be unique for each file.</li>
 <li>To pass a path using wildcards, it should be passed under quotes. e.g. 
 <pre>-f "home/dir1/*.log"</pre>
</ol>
  
  
  
Stop sending your file contents to Loggly

    sudo ./configure-file-monitoring.sh -a SUBDOMAIN -l FILE_ALIAS -r
