
## **🔐 File Permissions in Linux — Security & Access Control Project**

This project demonstrates how I analyzed and updated file and directory permissions within a Linux environment to align with organizational security requirements. The work was performed inside the `projects` directory, where several files and a subdirectory required permission adjustments to ensure proper authorization levels.

---

## **📌 Project Overview**

The research team needed to secure sensitive project files by ensuring that only the appropriate users and groups had access. I reviewed existing permissions, interpreted permission strings, and applied targeted changes using Linux commands. This process strengthened access control and reduced the risk of unauthorized modifications.

---

## **🧭 Tasks Performed**

### **1. Checked File and Directory Details**
- Used `ls -la` to list all contents of the `projects` directory, including hidden files.
- Identified:
  - One subdirectory: `drafts`
  - One hidden file: `.project_x.txt`
  - Five project files
- Reviewed the 10‑character permission string for each item to understand current access levels.

---

## **2. Interpreted the Linux Permission String**
Each permission string contains 10 characters:

| Section | Meaning |
|--------|---------|
| 1st character | File type (`d` = directory, `-` = file) |
| 2nd–4th | User permissions (read, write, execute) |
| 5th–7th | Group permissions |
| 8th–10th | Other permissions |

Example analyzed:  
`-rw-rw-r--` for `project_t.txt`  
- Regular file  
- User: read/write  
- Group: read/write  
- Other: read only  

This breakdown guided the permission changes that followed.

---

## **3. Updated File Permissions**
### **Removed Write Access for “Other”**
- The organization required that no file should allow write access to “other”.
- Updated `project_k.txt` by removing write permissions from other users.
- Verified changes using `ls -la`.

---

## **4. Modified Permissions on a Hidden File**
- `.project_x.txt` was archived and should no longer be modified.
- Requirements:
  - User: read only  
  - Group: read only  
  - Other: no access  
- Applied multiple `chmod` operations:
  - Removed write permissions from user and group  
  - Added read permission for group  

---

## **5. Restricted Directory Access**
- The `drafts` directory should only be accessible by the `researcher2` user.
- Removed execute permissions from the group.
- Ensured only the user retained execute access, preventing others from entering or listing the directory.

---

## **📌 Summary of Accomplishments**
- Audited existing permissions using `ls -la`.
- Interpreted permission strings to understand current access levels.
- Applied precise permission changes using `chmod` to:
  - Remove unauthorized write access  
  - Secure hidden files  
  - Restrict directory traversal  
- Ensured that file and directory permissions aligned with organizational security policies.

---

## **💡 Skills Demonstrated**
- Linux command-line navigation  
- File system permission analysis  
- Use of `ls`, `chmod`, and hidden file handling  
- Understanding of user, group, and other access levels  
- Practical application of least‑privilege security principles  

---



