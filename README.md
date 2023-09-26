# FileAccessPro

**Developer:** Manny Guerrero  
**Email:** mmguerrero1995@gmail.com
**LinkedIn:** https://www.linkedin.com/in/manny-g-933970263/
**Date:** September 26, 2023  
**Version:** 0.2.0
**Status:** Alpha / Development Stage

---

## ⚠️ Warning

This application is currently in its alpha/development stage. While we strive to develop a robust and secure file encryption tool, the application may contain bugs that could potentially lead to loss of data. 

**Users are solely responsible for any files that become irrecoverable due to use or misuse of FileAccessPro. It is highly recommended to exercise caution when using the application in its current state, including maintaining backups of all files to be encrypted or decrypted.**

We appreciate your understanding and welcome feedback and reports of any issues you encounter during use.

---

## What's New in Version 0.2.0

**New Features:**
- **User Account Support:** Added a backend SQLite database to support the use of user accounts. 
  - *Create Account:* Users now have the option to create an account by providing an email and password. Passwords are securely stored as hashes.
  - *Logged In State Tracking:* Application can now track if and which user is currently logged in.
  - *File Metadata Storage:* When a logged in user encrypts a file, the encryption data for that file is stored securely as hashed data in the encrypted_files table. Similarly, when a file is decrypted by a logged in user, the entry for that file is deleted from the encrypted_files table.

---

## Overview

FileAccessPro is an open-source, free-to-use desktop application designed to offer robust file encryption and decryption solutions with password protection. Safeguard your files with heightened security right from your desktop.

## Features

- **File Encryption/Decryption:** Securely encrypt your files with a password of your choice. Decrypt them back whenever you need.
- **Batch Processing:** Encrypt or decrypt multiple files at once, a feature that offers convenience and saves time.
- **Drag and Drop:** Easily add files for encryption or decryption using a drag-and-drop interface.
- **Custom File Extensions:** Encrypted files are given a custom extension to prevent double encryption and facilitate easy identification.
- **Graphical User Interface (GUI):** A user-friendly GUI built with PyQt6 for seamless user experience.

## How to Use

1. **Download and Install:** Clone the repository or download the source code and set up the necessary Python environment.
2. **Open the Application:** Run the `file_access_pro.py` script to open the application.
3. **Adding Files:**
    - **Browse:** Use the 'Browse' button to select files from your file system.
    - **Drag and Drop:** Simply drag and drop the files into the designated area in the application.
4. **Encryption/Decryption:**
    - **Encrypt:** After adding the files, click on the 'Encrypt' button, enter a secure password, and the files will be encrypted.
    - **Decrypt:** To decrypt, add the encrypted files, click on the "Decrypt" button, and enter the correct password.
        - **Note**: When decrypting multiple files in a batch, ensure all files were encrypted with the same password.

5. **View Encrypted Files:** Encrypted files will have a custom extension. You can find them at the same location as the original files.

---

## Future Features

We aim to continually evolve FileAccessPro to meet user demands and enhance functionality. Here are some prospective features we are considering for future versions:

- **Optional Write Destination:** Allow users to choose a specific destination where the encrypted/decrypted files will be saved.
- **Multiple Account Support:** Introduce an account system to facilitate batch encryption/decryption processes through a single login password, negating the need to enter a password for each batch. Initially, this feature will be local only.
- **Cloud Support:** Extend the functionality to support cloud services, enabling users to encrypt/decrypt files across different devices and integrate with popular cloud storage solutions like Dropbox and Google Drive.
- **Modernized GUI:** Update and modernize the appearance of the interface to improve the user experience.

## Contributing

As an open-source project, we welcome contributions from individuals and communities alike. Feel free to fork the repository and submit your contributions through pull requests.

## License

This project is open-source and free-to-use under the [MIT License](https://opensource.org/licenses/MIT).

---

We hope FileAccessPro serves you well in securing your files. For any queries or support, feel free to open an issue in the repository.
