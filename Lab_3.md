
Question

Use Vim,nano, to edit the editing_final_lab.txt file. Use the 
lab_file shell variable. Enter the visual mode of Vim. Remove 
the last seven characters from the first column on the first 
line. Preserve only the first four characters of the first 
column.

Step1:
 Preparing the Lab File
Ensure the file editing_final_lab.txt exists. If not, create it using:
touch editing_final_lab.txt
To simplify file access, store its path in a shell variable:
lab_file="editing_final_lab.txt"

Step2:
Editing with Nano
Nano is a beginner-friendly text editor.
Steps:
Open the file in Nano:
nano $lab_file
![image](https://github.com/user-attachments/assets/e6849054-8d45-489c-94ce-5abec35c0bb2)
![image](https://github.com/user-attachments/assets/3f91107a-f7d7-4a5b-88b0-f51d82120b8b)


Step3:
Editing with Vim
Vim is a powerful text editor with advanced features.

Steps:
Open the file in Vim:
vim $lab_file
Delete the Last Seven Characters of the First Line:
Enter visual mode (v), highlight the last seven characters, and press d.
Keep Only the First Four Characters of the First Line:
Move to the start of the line, press 4l, enter visual mode (v), highlight the rest, and press d.
Save and exit:
Press ESC, type :wq, and press Enter.


![image](https://github.com/user-attachments/assets/c241a021-190e-42b0-a173-fa52edc8d753)
![image](https://github.com/user-attachments/assets/4a30ef9d-e4b8-4fd6-9d5e-ecd7dbc17b58)

Step4:
Verifying Command Execution
To confirm the changes, display the file's contents:
![image](https://github.com/user-attachments/assets/c9f816df-ebec-47c8-a1ae-b9e8bf68d341)

Conclusion:
In this lab, you learned how to:

Use Nano for basic file editing.
Use Vim for advanced text manipulation, including deleting specific characters and retaining selected portions 
