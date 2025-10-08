# Yet another vulnerable web application
### This buggy web application contains vulnerability such as sqli,xss,access control vulnerabilities,IDOR etc and built with low to medium security to enhance the knowledge of script kiddies
### Default username and password for Admin login email ara@gmail.com password araara
## Set it up using the guide below
---

# 🐧 LAMPP (Linux)

1. **Start LAMPP**

   ```bash
   sudo /opt/lampp/lampp start
   ```

2. **Copy PHP Files**

   * Place your `.php` files into the LAMPP web directory:

     ```bash
     sudo cp -r /path/to/your/php-files/* /opt/lampp/htdocs/newsportal/
     ```
   * Access them at:
     👉 `http://localhost/newsportal/`

3. **Import Database via phpMyAdmin**

   * Open: 👉 [http://localhost/phpmyadmin/](http://localhost/phpmyadmin/)
   * Click **Databases** → Create new DB (name: `news`).
   * Select `news` → **Import** tab.
   * Browse and upload `news.sql`.
   * Click **Go** → schema + data imported.

4. **Update PHP Config**
   Inside your PHP connection file (e.g., `config.php`):

   ```php
   $servername = "localhost";
   $username   = "root";
   $password   = "";
   $dbname     = "news";
   ```

   (LAMPP root has no password by default.)

---

# 🪟 XAMPP (Windows)

1. **Start XAMPP**

   * Open **XAMPP Control Panel**.
   * Start **Apache** and **MySQL**.

2. **Copy PHP Files**

   * Place your `.php` files into:

     ```
     C:\xampp\htdocs\newsportal\
     ```
   * Access them at:
     👉 `http://localhost/newsportal/`

3. **Import Database via phpMyAdmin**

   * Open: 👉 [http://localhost/phpmyadmin/](http://localhost/phpmyadmin/)
   * Click **Databases** → Create new DB (name: `news`).
   * Select `news` → **Import** tab.
   * Browse and upload `news.sql`.
   * Click **Go** → schema + data imported.

4. **Update PHP Config**
   In your PHP connection file:

   ```php
   $servername = "localhost";
   $username   = "root";
   $password   = "";
   $dbname     = "news";
   ```

   (XAMPP root also has no password by default.)

---

