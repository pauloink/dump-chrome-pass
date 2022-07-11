# Installation:
Check for dependencies on requirements.txt

# First function:
### def chrome_date_and_time(chrome_data):
The **chrome_date_and_time()** function is responsible for converting Chrome’s date format into a human-readable date and time format.

# Second function:
### def fetching_encryption_key():
The **fetching_encryption_key()** function obtains and decodes the AES key used to encrypt the password. It is saved as a JSON file in “C:\Users\<HOME_DIR>\AppData\Local\Google\Chrome\User Data\Local State”. This function will be useful for the encrypted key.

# Third Function
### def password_decryption(password, encryption_key):
**password_decryption()** takes the encrypted password and AES key as parameters and returns the decrypted version or Human Readable format of the password.

# Output example:
![](https://i.imgur.com/QBbqdhs.png)

# Steps
- First, we use the previously defined function fetching_encryption_key() to obtain the encryption key
- Then copy the SQLite database in “C:\Users\<HOME_DIR>\AppData\Local\Google\Chrome\User Data\default\Login Data” where the saved Password data is stored of the current directory and establish a connection with it. This is because the original database file locked when Chrome started. 
- With the help of the cursor object, we will execute the SELECT SQL query from the ‘logins’ table order by date_last_used.
- Traverse all the login rows in a more readable format to obtain the passwords for each password and format date_created and date_last_used.
- Finally, With the help of print statements, we will print all the saved credentials which are extracted from Chrome.
- Delete the copy of the database from the current directory.
