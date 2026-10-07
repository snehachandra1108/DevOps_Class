## Task 1: Soft Link & Hard Link
- Learn the difference between soft links and hard links.
- Learn the commands to create both.
- Practice creating and deleting soft and hard links.
- Prepare for this as an interview question.


### Soft Link

A **soft link (symbolic link)** is a file that points to another file. It acts as a shortcut to the original file.

#### Command to create a soft link :

```bash
ln -s file1.txt softlink.txt
```
Here:

- ln → creates a link
- -s → creates a symbolic (soft) link
- file1.txt → original file
- softlink.txt → name of the soft link

### Hard Link

A **hard link** is another name/link for an existing file. Both the original file and the hard link refer to the same underlying data.

#### Command to create a hard link :

```bash
ln file1.txt hardlink.txt
```
Here:

- ln → creates a link
- file1.txt → original file
- hardlink.txt → name of the hard link
### Deleting Links

```bash
rm softlink.txt
rm hardlink.txt
```
### What is the difference between a soft link and a hard link?

A soft link is like a shortcut that points to the path of another file, whereas a hard link is another link to the same underlying file. If the original file is deleted, a soft link becomes broken, while a hard link can still access the file.

### Screenshots :

Creating soft link :
<img width="1075" height="335" alt="image" src="https://github.com/user-attachments/assets/30180a50-bcec-406c-8216-19c9df272078" />

Creating hard link :
<img width="952" height="176" alt="image" src="https://github.com/user-attachments/assets/6ebff235-4421-49ed-a589-43d7291b3d8e" />

Deleting links :
<img width="957" height="121" alt="image" src="https://github.com/user-attachments/assets/7e5f8bb6-309e-419e-b29d-28525e47d72f" />

## Task 2: adduser vs useradd
- Learn the difference between adduser and useradd.
- Understand which command is preferred on Ubuntu/Linux and why.
- Create a test user using the recommended command.
##

Linux provides two commonly used commands for creating users:
- **adduser**
- **useradd**
Both are used to create users, but they differ in how they work and how much configuration they handle automatically.

### adduser

**adduser** is a user-friendly and interactive command for creating a new user.
It guides the user through the creation process and automatically handles common tasks such as creating the user's home directory and setting up the user.

#### command :

```bash
sudo adduser testuser
```
### useradd

**useradd** is a lower-level command for creating users.
It is less interactive and usually requires additional options when configuring the user's home directory,password, etc.

#### command :

```bash
sudo useradd testuser
```
### Which command is preferred on Ubuntu?

**adduser** is generally preferred when creating users manually on Ubuntu because it is interactive and handles common user setup automatically.
**useradd** is useful when more control is required.

### Screenshots :

Creating testuser :

<img width="745" height="483" alt="image" src="https://github.com/user-attachments/assets/a2949779-caf9-4505-b83d-6894aed5c2d7" />

Switching to testuser :

<img width="747" height="220" alt="image" src="https://github.com/user-attachments/assets/7e1c0b3b-d784-4790-bca1-e4a8b02b9f0b" />

## Task 3: journalctl
- Learn what journalctl is used for.
- Learn how to view system and service logs using journalctl.
- Practice checking logs for a specific service.

##

### What is journalctl?

**journalctl** is a linux command used to view and examine system and service logs.

Logs provide information about events happening on the system, such as:
- Services starting or stopping
- System startup and shutdown
- Errors and warnings
- Other system activities

### Viewing logs

To view system logs:
```bash
journalctl
```
To view ssh service logs:
```bash
journalctl -u ssh
```

### Screenshots :

System logs :

<img width="1838" height="511" alt="image" src="https://github.com/user-attachments/assets/ccc990ca-cea4-40da-b375-580d190f6366" />

Service logs :

<img width="590" height="51" alt="image" src="https://github.com/user-attachments/assets/fba1bd77-3179-45ea-bc97-a66b0ca87cf8" />

## Task 4:Linux Command Cheat Sheet
- Review the Linux command cheat sheet.
- Practice the important commands covered in the cheat sheet.
- Understand the purpose and basic usage of each command.

##

### Screenshots :
<img width="1796" height="1093" alt="image" src="https://github.com/user-attachments/assets/0be51693-5dcd-47d7-91d1-bc7d6df3f454" />

<img width="1796" height="1093" alt="image" src="https://github.com/user-attachments/assets/2ae1c452-9b21-4e5c-9f58-49ed9b2b31e1" />


