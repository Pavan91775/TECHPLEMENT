# TECHPLEMENT_TASK

Commands

1. Install apache server on Ubuntu
   
**sudo apt install apache2**

3. Install php runtime and php mysql connector
   
**sudo apt install php libapache2-mod-php php-mysql**

5. Install MySQL server
   
**sudo apt install mysql-server**

7. Login to MySQL server
   
**sudo mysql -u root**

9. Change authentication plugin to mysql_native_password (Choose strong password)
    
**ALTER USER 'root'@'localhost' IDENTIFIED BY 'bablu123456';**  

11. Create a database for wordpress
    
**CREATE DATABASE bablu_db;**

13. Create a new database user for wordpress
    
**CREATE USER 'bablu_user'@localhost IDENTIFIED BY 'bablu123456';**


15. Grant all privileges on the database 'wordpress' to the newly created user
    
***GRANT ALL PRIVILEGES ON bablu_db.* TO 'bablu_user'@'%';**
**FLUSH PRIVILEGES;**

17. Download wordpress
    
**cd /tmp wgethttps://wordpress.org/latest.tar.gz**

19. Unzip the file
    
**tar -xvf latest.tar.gz**

21. Move Wordpress folder to apache document root
    
**sudo mv wordpress/ /var/www/html**

23. Command to restart apache server
**sudo systemctl restart apache2**
