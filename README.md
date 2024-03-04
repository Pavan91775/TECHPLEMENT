# TECHPLEMENT_TASK

Commands
1. Install apache server on Ubuntu
   
   > **sudo apt install apache2**

2. Install php runtime and php mysql connector
   
   > **sudo apt install php libapache2-mod-php php-mysql**

3. Install MySQL server
   
   > **sudo apt install mysql-server**

4. Login to MySQL server
   
   > **sudo mysql -u root**

5. Change authentication plugin to mysql_native_password (Choose strong password)
    
   > **ALTER USER 'root'@'localhost' IDENTIFIED BY 'bablu123456';**  

6. Create a database for wordpress
    
    > **CREATE DATABASE bablu_db;**

7. Create a new database user for wordpress
    
    > **CREATE USER 'bablu_user'@localhost IDENTIFIED BY 'bablu123456';**


8. Grant all privileges on the database 'wordpress' to the newly created user
    
    > **GRANT ALL PRIVILEGES ON bablu_db.*** **TO 'bablu_user'@'%';**
    
    > **FLUSH PRIVILEGES;**

9. Download wordpress
    
    > **cd /tmp wgethttps://wordpress.org/latest.tar.gz**

10. Unzip the file
    
    > **tar -xvf latest.tar.gz**

11. Move Wordpress folder to apache document root
    
    > **sudo mv wordpress/ /var/www/html**

12. Command to restart apache server
    
    > **sudo systemctl restart apache2**
