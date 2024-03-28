# Sticky-Situation

# Scenorio
A highly confidential document has been stolen from the President's laptop and has been sold on the Dark Web. The Secret Service thinks someone with physical access to the laptop was able to retrieve the important document, and they suspect the likely method was ATT&CK ID T1052.001. Can you help the Secret Service to figure out how this happened?

# Tools
- Autopsy.
- Window File Analyzer.
- WinPrefetchView.
- Jumplist Explorer.

# QUESTION 1
* What is the computer name?
To determine the name of the computer, we initially import the documents into Autopsy. Once imported, we navigate to "Operating System Information" where the computer name will be identifiable.
<img width="901" alt="Screenshot 2024-03-26 at 22 36 35" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/98db2409-6a28-438e-9b82-2df6627cf23e">

# QUESTION 2 
* When was the OS installed?
To ascertain the installation date of the OS, we move to the right in the same window and seek out "Date/Time." Here, the installation date will be visible.
<img width="889" alt="Screenshot 2024-03-26 at 22 43 58" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/cae2cc90-58a4-427f-ba42-4407934f9e9b">

# QUESTION 3
* What is the Timezone of the computer?
To determine the time zone, proceed to Desktop > Investigation > Sticky Situation > Module Output > Recent Activity > Registry > SYSTEM - regripper-565982. Within the system registry, use search terms such as "tz" or "timezone" to pinpoint the specific information needed.
<img width="894" alt="Screenshot 2024-03-26 at 23 04 13" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/e86b574b-7ea0-49ee-9436-0c385d7fcea1">

# QUESTION 4
* What is the serial number of the first USB mass storage device connected?
To find the serial number of the initial USB mass storage device connected, return to Autopsy and access "USB devices attached". Arrange the dates in descending order, simplifying the process of identifying the serial number.
<img width="1364" alt="Screenshot 2024-03-27 at 20 21 55" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/65e75783-355e-4a3d-b01e-6afe235407c8">

# QUESTION 5
* What is the vendor name of the first USB mass storage device?
In the same window, you can locate the vendor's name under the "Device Make" column.
<img width="1356" alt="Screenshot 2024-03-27 at 20 29 00" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/fe0bd3de-5986-4531-a735-42f6dcf2f22f">

# QUESTION 6
* When was the first USB mass storage device connected for the first time?
To determine the date and time when the first USB mass storage device was initially connected, we navigate to the system file and search using the USB's serial number. This will reveal the exact moment the USB device was connected.
<img width="1339" alt="Screenshot 2024-03-27 at 21 06 57" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/3a002694-fa46-401f-be11-69ca1dd93e90">

# QUESTION 7
* What is the Volume Label of the unique USB mass storage device?
To identify the Volume Label of the specific USB mass storage device, navigate to the software file within the investigation folder and conduct a search using the USB's serial number. Upon locating the serial number, the volume label associated with it can be found.
<img width="1349" alt="Screenshot 2024-03-27 at 21 15 34" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/81ddb3d6-6a63-4b97-b094-68bc20a8cc06">

# QUESTION 8
* Find the user that used the USB Device. What is the user’s SID?
To discover which user utilized the USB device and obtain the user's Security Identifier (SID), proceed to the "operating system user account" section, identify the most recent date, and then copy the User ID.
<img width="1355" alt="Screenshot 2024-03-28 at 21 31 07" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/1a5d28b6-9ff7-4339-acfe-e35306745400">

# QUESTION 9
* What is the last drive letter assigned to the USB device?
To determine the last drive letter assigned to the USB, return to Autopsy and access the recent documents section. Search for the source path, which corresponds to the label of the unique USB mass storage device. Upon locating it, the last drive letter designated to the USB device will be visible.
<img width="1349" alt="Screenshot 2024-03-28 at 21 41 40" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/e4534acc-8a2b-4c9a-bc17-f0b08aac4c38">

# QUESSTION 10
* What is the filename of the document stolen?
In the "recent document folder," it is also evident that the document stolen is "finance.txt".
<img width="1333" alt="Screenshot 2024-03-28 at 21 52 54" src="https://github.com/AlCybx/Sticky-Situation/assets/161755166/ed0159d0-e964-4645-8f93-e8bd2f7b9e40">












