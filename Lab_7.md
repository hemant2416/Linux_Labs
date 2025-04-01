Experiment 7

Question:
Implement chown, chmod command with their options


Step1:
 Managing File Ownership with chown
The chown command is used to change the owner and/or group of files and directories.

a. Changing the Owner of a File
sudo chown operator1 testfile.txt
![image](https://github.com/user-attachments/assets/a043371a-83ed-4053-ac55-34bd550b572d)

b. Changing Both Owner and Group
sudo chown operator1:operator2 testfile.txt
![image](https://github.com/user-attachments/assets/3727cf7e-4064-4217-a423-aa87c41afc72)

c. Recursive Ownership Changes
sudo chown -R operator1:operator1 testdirectory/
![image](https://github.com/user-attachments/assets/a199d758-77fb-4d3b-9431-c23a7d6a7b7b)


Step2:
 Managing File Permissions with chmod
The chmod command is used to modify file access permissions for the owner, group, and others.

a. Setting Permissions Using Numeric Mode (Octal)

1.Assign read, write, and execute permissions to the owner only:
chmod 700 testfile.txt
Explanation: Owner gets full permissions (7), group and others get none (0).

2.Assign read and write for the owner, and read-only for group and others:
chmod 644 testfile.txt

![image](https://github.com/user-attachments/assets/0f407fec-eac9-40b5-b721-47d5876a23aa)

b. Setting Permissions Using Symbolic Mode

1.Add execute permission for the owner:
chmod u+x testfile.txt

2.Remove write permission for the group:
chmod g-w testfile.txt

3.Add read permission for others:
chmod o+r testfile.txt

4.Set multiple permissions at once:
chmod u+rwx,g+rx,o+r testfile.txt

![image](https://github.com/user-attachments/assets/aa4d9a21-4359-4f1e-966b-470bc7e034b4)


Conclusion:
In this lab, you practiced:

Changing file and directory ownership using chown.
Modifying file and directory permissions using chmod.
Applying recursive changes and special permissions (SUID, SGID, Sticky Bit).
Verifying permission and ownership changes.
