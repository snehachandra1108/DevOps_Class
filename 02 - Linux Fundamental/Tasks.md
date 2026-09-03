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
