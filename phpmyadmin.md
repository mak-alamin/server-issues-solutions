
## Maximum execution time exceeded issue

### Solution:
### Add this line to xampp\phpmyadmin\config.inc.php (for ubuntu /usr/share/phpmyadmin/libraries/config.default.php)

$cfg['ExecTimeLimit'] = 6000;


### And Change xampp\php\php.ini to

post_max_size = 750M 

upload_max_filesize = 750M   

max_execution_time = 5000

max_input_time = 5000

memory_limit = 1000M


### And change xampp\mysql\bin\my.ini

max_allowed_packet = 200M
