![Screenshot 2025-06-29 002033](https://github.com/user-attachments/assets/540fec83-9b2a-4924-b1b6-9fd15aea9c22)

![Screenshot 2025-06-29 002156](https://github.com/user-attachments/assets/ef237a79-0262-4a4d-8150-ccb4deb673d0)


![Screenshot 2025-06-29 002222](https://github.com/user-attachments/assets/63949b4e-4a68-4020-8e76-66940323bae3)

# Simple Linux Backup Script

This is a simple bash script that helps you back up files from one directory to another on Linux.

## What it does

* Asks you for a **source directory** (the folder you want to back up).
* Asks you for a **destination directory** (where you want the backup to go).
* Uses `rsync` to copy all files and keep them in sync.
* Shows a message when the backup is complete.

## How to use

1. Make the script executable:

   ```bash
   chmod +x backup.sh
   ```

2. Run the script:

   ```bash
   ./backup.sh
   ```

3. Enter the source and destination paths when prompted.

## Example

* Source: `/home/kali/Desktop/test`
* Destination: `/home/kali/Desktop/test2`

The script will copy all files from `test` to `test2`.

## Note

* This script uses `rsync -av --delete` which means deleted files in the source will also be deleted in the destination on the next backup.
* Make sure `rsync` is installed on your system.

## License

Free to use and modify.
