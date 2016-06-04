# ionizecms_fixed_404_admin_page
solved the problem when ionize CMS admin page was not found

<b>step 1</b><br/>
Enable mod_rewrite for Apache<br/>
<i># a2enmod rewrite</i>
<br/><br/>
<b>step 2</b><br/>
/etc/apache2/sites-available/default.conf<br/>
/etc/apache2/sites-enabled/default.conf<br/>
Add<br/>
```html
<Directory /var/www/html/YOUSITEDIRRECTORY/>
                AllowOverride All
                Order Allow,Deny
                Allow from all
</Directory>
```
<br/><br/>
<b>step 3</b><br/>
Download and replace file .htaccess

<br/><br/>
<b>step 4</b><br/>
<i># /etc/init.d/apache2 restart</i>

<br/><br/>
<b>done ;)</b><br/>
