# ubiq_lib_encrypt_decrypt

# To Encrypt Some Simple Data:
**Enpoint:**\
http://localhost:8080/api/v1/ubiq/encrypt

**Request Type:** POST

**Request Body:**
{
    "input": "This text will be encrypted"
}

**Response Body:**
{
    "respCode": "00",
    "respDescription": "Success",
    "output":"encrypted data"
}

# To Decrypt Data:
**Endpoint:**\
http://localhost:8080/api/v1/ubiq/decrypt

**Request Type:** GET\
It will decrypt the previously encrypted data. So you need to first call encrypt endpoint before calling this endpoint.

# To Encrypt Data From File:
**Endpoint:**\
http://localhost:8080/api/v1/ubiq/encryptFile

**Request Type:** POST

**Request Body:**
{
    "inputFilePath": "D:/My_Folder/Dev_Library/IntelliJ/Other/ubiq/Input/input.txt",
    "outputFilePath": "D:/My_Folder/Dev_Library/IntelliJ/Other/ubiq/Output/encrypted/output.enc"
}

**Response:**\
Encrypted Successfully

# To Decrypt Data From Encrypted File:
**Endpoint:**\
http://localhost:8080/api/v1/ubiq/decryptFile

**Request Type:** POST

**Request Body:**
{
    "inputFilePath": "D:/My_Folder/Dev_Library/IntelliJ/Other/ubiq/Output/encrypted/output.enc",
    "outputFilePath": "D:/My_Folder/Dev_Library/IntelliJ/Other/ubiq/Output/decrypted/output.txt"
}

**Response:**\
Decrypted Successfully
