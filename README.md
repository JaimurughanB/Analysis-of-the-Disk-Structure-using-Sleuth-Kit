# Analysis-of-the-Disk-Structure-using-Sleuth-Kit
## AIM:
To analyze the disk structure of a given disk image using Sleuth Kit tools in Kali Linux.

## DESIGN STEPS:
### Step 1:
Obtain or create a disk image file (e.g., disk.dd) to analyze. Open the terminal in Kali Linux.

### Step 2:
Use Sleuth Kit tools like mmls, fsstat, and fls to examine the partition layout, file system details, and file listing.

### Step 3:
Interpret the output of the tools to understand the disk structure, including partitions, sectors, and files.

## PROGRAM:
Sleuth Kit Disk Analysis Commands✅ Option 1: Create a Sample Disk Image (for Testing)

Let’s create a 10MB blank disk image and simulate file system activity:
cd ~/Downloads

# Step 1: Create an empty disk image
dd if=/dev/zero of=disk.dd bs=1M count=10

# Step 2: Format it with a file system (like FAT32)
mkfs.vfat disk.dd

## OUTPUT:
![image](https://github.com/user-attachments/assets/c0943afd-b931-4811-8cdb-c1b750556b56)
## Create Disk:
![image](https://github.com/user-attachments/assets/20b2da8a-c556-4cd8-8211-88a62a7cb67e)
## mmls:
mmls disk.dd
## fls:
fls -f fat -o 0 disk.dd
![image](https://github.com/user-attachments/assets/e2942f8c-3ccf-486a-930f-f5695a7c32de)
![image](https://github.com/user-attachments/assets/ab510c13-e3b3-45a0-9ee8-dcf444be0578)
![image](https://github.com/user-attachments/assets/5db03141-b5e9-4ab3-92b9-84e16c621479)
![image](https://github.com/user-attachments/assets/ba2441cb-b65f-4b98-8a6e-bf1d4c007df5)


## RESULT:
The analysis was performed successfully using Sleuth Kit, and the disk structure was understood in detail.
