# SSis 
-- Design SSIS Package to transfer Department data From [ITI DB] to [Test Db]. 
Note “before transferring data to [Test db] try to truncate table department”



![transfer_department](https://github.com/user-attachments/assets/3e407ee2-cc12-465b-93a1-04552cd651d1)





-- Design SSIS Package to transfer Student data (St_id, St_Fname, St_lname, St_address) From [ITI DB] to new Delimited file “Student.txt” and set column name as the first row in the file.



![2](https://github.com/user-attachments/assets/53bc02e3-c45d-484a-a393-4bd7b1ee0033)





--Design SSIS Package to transfer Student data from [ITI DB] to [Test DB] with the following Criteria:
a-	If table Student Exists in [Test DB] delete all data. Use [Execute SQL Task Component]
b-	Merge the first name and last name to be one field [Full name]. use [Derived Column Component]
c-	Make a full backup for [Test DB]
d-	On error display message box “error occurred”

![3](https://github.com/user-attachments/assets/6d866554-2ff1-4852-8e43-7b38a0fe2878)           ![3-1](https://github.com/user-attachments/assets/4f20667a-9462-4836-b684-5475cfa85ebd)








4-	Design SSIS Package to Split Course data from [ITI DB] into 3 files with the following criteria:
a-	Select Course data with topic name From ITI DB
b-	Sort Course data by Crs_name Descending. use [Sort Component]
c-	Crs_name should appear in lower case. Use [Character Map Component] 
d-	Split Course data into 3 files:	
i.	File1.txt contains Course data with Course Duration<30 hours.
ii.	File2.txt contains Course data with Course Duration=30 hours.
iii.	File3.txt contains Course data with Course Duration>30 hours.
Note: set columns name as first row in the files



![4](https://github.com/user-attachments/assets/e742cb0c-2cc0-4e7a-896f-5c058c4853bc)



merge the file1.txt and file2.txt to be one file:
a-	Use [Merge Component]. “Sort by Crs_name”
b-	Use [Union Component]

![5-1](https://github.com/user-attachments/assets/df2c204c-de4c-4dc2-88ff-e3e4243244c6)
![5](https://github.com/user-attachments/assets/47411bef-1901-480f-92e8-d7cb5f150d53)









