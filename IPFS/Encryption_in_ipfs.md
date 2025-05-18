## Perform encryption and privacy on IPFS through command line.  
### IPFS privacy and encryption
- ``echo "Hello, IPFS!" > myfile.txt``
- ``` ipfs add myfile.txt ```
- ``` openssl enc -aes-256-cbc -pbkdf2 -iter 100000 -salt -in myfile.txt -out myfile_encrypted.txt -pass pass:yourpassword```
- ``` ipfs add myfile_encrypted.txt ```
- ``` cat myfile_encrypted.txt ```
- ``` openssl enc -d -aes-256-cbc -pbkdf2 -iter 100000 -in myfile_encrypted.txt -out decrypted_file.txt -pass pass:yourpassword ```
- ```cat decrypted_file.txt```
- ``` ipfs add decrypted_file.txt ```
