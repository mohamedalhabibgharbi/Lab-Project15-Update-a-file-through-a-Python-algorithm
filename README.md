# 🔐 Update a file through a Python algorithm (Goolge Cybersecurity Professional Certificate Project) 

## 📝 Project description  
In my organization, we control access to restricted content using a list of approved IP addresses. The allow_list.txt file contains these IP addresses. There's also a separate list that includes IP addresses that should be blocked from accessing this content. I created a program to automatically update the allow_list.txt file by removing the IP addresses that are no longer allowed access.

---

## 📂 Open the file that contains the allow list  
For the first part of the algorithm, I opened the allow_list.txt file. First, I assigned this file name as a string to the import_file variable:  
![Screenshot1](https://i.imgur.com/aGQ6CID.png)

Then, I used a with statement to open the file:  
![Screenshot2](https://i.imgur.com/0WEZvt2.png)

---

## 📖 Read the file contents  
In order to read the file contents, I used the .read() method to convert it into a string.  
![Screenshot3](https://i.imgur.com/WQWY4v1.png)

---

## 🔁 Convert the string into a list  
In order to remove individual IP addresses from the allow list, I needed it to be in list format. Therefore, I next used the .split() method to convert the ip_addresses_string into a list:  
![Screenshot4](https://i.imgur.com/AMbRjwi.png)

---

## 🔍 Iterate through the remove list  
A key part of my algorithm involves iterating through the IP addresses that are elements in the remove_list. To do this, I incorporated a for loop:  
![Screenshot5](https://i.imgur.com/n2BW7hf.png)

---

## 🧹 Remove IP addresses that are on the remove list  
My algorithm requires removing any IP address from the allow list, ip_addresses, that is also contained in remove_list.  Because there were not any duplicates in ip_addresses, I was able to use the following code to do this:  
![Screenshot6](https://i.imgur.com/b2p6Bvu.png)

---

## 💾 Update the file with the revised list of IP addresses  
As a final step in my algorithm, I needed to update the allow list file with the revised list of IP addresses. To do so, I first needed to convert the list back into a string. I used the .join() method for this:  
![Screenshot7](https://i.imgur.com/SxEB1el.png)

Then, I used another with statement and the .write() method to update the file:  
![Screenshot8](https://i.imgur.com/FteS8sQ.png)

---

## ✅ Summary  
I created an algorithm that removes IP addresses identified in a remove_list variable from the allow_list.txt file of approved IP addresses. This algorithm involved:  
• Opening the file  
• Converting it to a string to be read  
• Converting this string to a list stored in the variable ip_addresses  
• Iterating through the IP addresses in remove_list  
• Removing matches from the list  
• Converting the list back into a string using .join()  
• Writing the updated content back to the file
