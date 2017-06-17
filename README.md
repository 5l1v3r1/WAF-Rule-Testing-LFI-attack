# WAF-Rule-Testing (Local File Inclusion-LFI Rules)
Testing Local File Inclusion (LFI)  attack on vulnerable application with OWASP CRS && CWAF Ruleset 1.127 (latest version). 

**Testing LFI attack on OWASP CRS**
    
     Include the OWASP CRS on apache config:
     #REQUEST-930-APPLICATION-ATTACK-LFI
     #PARANOIA_LEVEL:1
     #rule ID:930100,930110,930120,930130
    
     Test these following payloads on the xvwa vulnerable application for Local File Inclusion (LFI) attack.
     
        /var/mail/www-data
        /etc/network/* i.e /etc/network/interfaces
        /etc/init/* i.e /etc/init/anacron.conf
    
     As a result, OWASP CRS failed to block the user from accessing the above sensitive path or file, but it block almost ever major LFI attacks. 
     
     Check the demo video to know more :)
 
 **Testing LFI attack on CWAF Ruleset**
    
     Include the CWAF ruleset on apache config:
     
     Test these following payloads on the xvwa vulnerable application for Local File Inclusion (LFI) attack.
        /var/mail/www-data
        /usr/share/apache2/* i.e /usr/share/apache2/build/config.nice
        /usr/share/php5/mysql/mysql.ini

      As a resut, CWAF failed to block the user from accessing the above sensitive path or file, but it block all other LFI attack on application and it show FP on LFI payloads.
      
      Check the demo video to know more :)
      
## Demo Video
  
   [![Alt text](https://img.youtube.com/vi/dU9pShTKq_w/0.jpg)](https://www.youtube.com/watch?v=dU9pShTKq_w)

## Support !
 Email address: umarfarookmech712@gmail.com  for more details. <br>
 Youtube: [FOS](https://www.youtube.com/channel/UCEBHO0kD1WFvIhf9wBCU-VQ) <br>
 Blog: [FOS](https://fosecurity.blogspot.com) 

## Useful links:
 1. [Modsecurity](www.modsecurity.com/)
 2. [Kali](https://www.kali.org/)
 3. [Debuggex](https://www.debuggex.com/)
 4. [OWASP Mutillidae Vulnerable App](https://www.owasp.org/index.php/OWASP_Mutillidae_2_Project)
 5. [XVWA](https://github.com/s4n7h0/xvwa)

