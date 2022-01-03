Documentation available for all the sites under ciges.net

Add the following Alias to VirtualHost Apache configurarion to have it available

In the example the repository is downloaded on /home/ciges/webs/docs 

```apacheconf
    # Alias to directories outside the DocumentRoot
    # CV under docs
    Alias /docs /home/ciges/webs/docs
    # Demo of RevealJS
    Alias /revealjs_demo /home/ciges/webs/docs/revealjs_demo
    # PHPdoc for IntenetAccessLog (2012 Software Libre Master)
    Alias /phpdoc /home/ciges/webs/docs/phpdoc
    <Directory /home/ciges/webs/docs>
        Options Indexes FollowSymLinks
        AllowOverride All 
        Require all granted
        Order allow,deny
        Allow from all
     </Directory>
```
