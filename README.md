# 1/ Context

I have been helping my father because he could not update his PC to Windows 11.

I felt it would be best to share it as this is not straight forward for anyone not willing to dig for something which should be straight forward.

# 2/ Update Status 

First step I would suggest it to install Windows 11 [**PC Health Check app**](https://support.microsoft.com/en-us/windows/check-if-a-device-meets-windows-11-system-requirements-after-changing-device-hardware-f3bc0aeb-6884-41a1-ab57-88258df6812b): 
<img width="436" height="313" alt="image" src="https://github.com/user-attachments/assets/596e2c19-714d-41a2-b860-8e60ec38ad90" />

This will explain what is currently blocking the update to Windows 11. In my case, it was because of the CPU which is a non sense.

# 3/ Disk Usage

After that, I would recommend a check of the disk usage (64GB should be available).

[**Windirstat**](https://windirstat.net/) is very good and clear for that (click and remove personal files, for system files, check online first):
<img width="952" height="511" alt="image" src="https://github.com/user-attachments/assets/529afbd9-9dc5-4a6f-9bce-e3459d24b5e2" />

# 4/ Cleaning

Another intersting software is [**PatchCleaner**](https://sourceforge.net/projects/patchcleaner/) to remove unused system files (MSP for example, I had 50GB of them):
<img width="713" height="253" alt="image" src="https://github.com/user-attachments/assets/6f01ac5e-8bf9-4f7c-adf2-66c32120d64c" />

I would also recommend to remove any old application you don't use from [**All Apps**](https://support.microsoft.com/en-us/windows/uninstall-or-remove-apps-and-programs-in-windows-4b55f974-2cc6-2d2b-d092-5905080eaf98) menu. 

From there, the system should be a bit cleaner for the update.

# 5/ Windows 11 Update

Last step is to download [**Windows 11**](https://www.microsoft.com/en-us/software-download/windows11) iso file to be able to bypass the hardware checks.

When the ISO is download, doulbe click on it to mount it, it will appear as a Drive (for example F:).

Open a command line terminal by searching for **cmd** application in the search bar.

From this terminal, go to the mounted disk by typing **F:** (assuming F is the mounting drive selected by the system).

Finally, type this command to start the installation without the hardware check (from there, it is the standard graphical interface of Windows 11 installation):
```
setup.exe /product server
```
