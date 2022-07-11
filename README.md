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
