# Robocopy
Tags: #robocopy
Author: Shahid Sharif
Initial Release: 22Mar2021
Last Update:  22Mar2021-04:00
Reference: [How to Run Robocopy Two-Way Sync for Folders in Windows 10/8/7? (ubackup.com)](https://www.ubackup.com/synchronization/robocopy-two-way-sync-8523.html)

---

```python
@echo OFF
echo Syncing from C drive to E drive
robocopy e:\Data f:\Data /e /z 
echo Syncing from E drive to C drive
robocopy "E:\\synced files" "C:\\Users\\AOMEI Technology\\Documents" /e /z
echo Sync Complete
pause
 ```