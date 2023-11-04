## Instllations
[Postman](https://www.postman.com)
[VSCode](https://code.visualstudio.com)

```bash
# Virtual Environment
# Install Development Tools:
sudo apt-get install build-essential libssl-dev libffi-dev python-dev
# Install pip:
sudo apt-get install -y python3-pip
# Install Virtualenv:
sudo pip3 install virtualenv
# # Install venv Module:
# sudo apt-get install -y python3-venv
# Create Virtual Environment Using Python3:
virtualenv -p python3 blog 
# Activate Virtual Environment:
source venv/bin/activate
# Install The Requirements:
pip install -r requirements.txt
```

```bash
# Install cURL
sudo apt update
sudo apt install curl
curl --version
```

```bash
# Install SQLite
# Update your package list:
sudo apt update
# Install SQLite:
sudo apt install sqlite3
# Verify the installation:
sqlite3 --version
```

```bash
# Install MySQL
# Update the package index:
sudo apt update
# Install the mysql-server package:
sudo apt install mysql-server
# Ensure that the server is running using the systemctl start command:
sudo systemctl start mysql.service
# Open up the MySQL prompt
sudo mysql
# Change the root user’s authentication method to "mysql_native_password" one that uses a password:
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'password';
# Exit the MySQL prompt:
exit
# Secure MySQL installation:
sudo mysql_secure_installation
# Open MySQL as root:
mysql -u root -p
# Create new user:
CREATE USER 'alansary'@'localhost' IDENTIFIED WITH mysql_native_password BY '123456';
# Create database:
CREATE DATABASE blog;
# Give user privileges to the database:
GRANT ALL PRIVILEGES ON blog.* TO 'alansary'@'localhost';
# Free up any memory that the server cached as a result of the preceding CREATE USER and GRANT statements:
FLUSH PRIVILEGES;
# Exit the MySQL client
exit
# Connect to MySQL using the new user:
mysql -u alansary -p
```