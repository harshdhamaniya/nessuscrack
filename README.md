# Nessus Crack 2023 - 32 IPs Bypass - Unlimited IP Scan - Harsh Dhamaniya
---

## Download and Install Nessus

![Untitled 1](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/473209a1-278e-4a62-8a75-e9aaf74077b2)


## Install Nessus (Default Location)

![Untitled 2](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/86830874-da06-48af-a695-8ad36fa1eec0)

![Untitled 3](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/2134a3f9-7d83-458c-8212-9c51f33a541b)


### Setup Nessus Free or Professional With a Key (Using NessusKeygen by Harsh Dhamaniya)

```jsx
git clone "https://github.com/harshdhamaniya/nessuskeygen"
cd nessuskeygen
python nessuskeygen.py
Enter 1 and copy key
```

![Untitled 4](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/a941a8ae-1d9b-4bc2-9687-f51ad03881d9)


### On This Window

![Untitled 5](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/1429a724-6fa4-420b-953f-f2cd6bf3f8c9)


# Adding User to Nessus

### Open a CMD Window with Admin Rights and Enter the following commands

```jsx
cd cd "C:\Program Files\Tenable\Nessus"
nessuscli adduser

**Form Details**
Login : admin
Login password: admin
Login password (again): admin
Do you want this user to be a Nessus 'system administrator' user (can upload plugins, etc.)? (y/n) [n]: y
(Make sure to type y)
Press Enter When asked rules
This user will have 'system administrator' privileges within the Nessus server
Is that ok? (y/n) [n]: y
(Make sure to type y)
```

![Untitled 6](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/6c7f3f78-84bc-44c9-90ac-e3d1a7f86114)


### Run the following commands in CMD Window

```jsx
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
```

- If you face error “File not found” then create a file named “plugin_feed_info.inc” in "C:\ProgramData\Tenable\Nessus\nessus\” Folder.

### Download the Plugin File using the below mentioned link

[Download Plugin - Click Here](https://plugins.nessus.org/v2/nessus.php?f=all-2.0.tar.gz&u=56b33ade57c60a01058b1506999a2431&p=1ee9c89d5379a119a56498f2d5dff674)

### Goto the following Directory and run the following command

```jsx
cd "C:\Program Files\Tenable\Nessus"
nessuscli update <Location of all-2.0.tar.gz>
example : nessuscli update "C:\Users\Harsh Dhamaniya\Downloads\all-2.0.tar.gz"
```

`If You’re Unable to Locate just paste it in the run (Win+R)`

![Untitled 7](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/6d6e0cf8-6bdc-44d0-a197-7303047b560b)


As you can see we have 32 IPs Limit, Lets Bypass it.

![Untitled 8](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/e4d91486-91d1-4581-8d65-643c2b40a39a)


### Goto Plugins Folder and edit/create a file named plugin_feed_info.inc

![Untitled 9](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/fa0d7dde-5a72-4376-8164-229f693ed24a)


### Write the following lines in that file

```jsx
PLUGIN_SET = "202309091407";
PLUGIN_FEED = "ProfessionalFeed (Direct)";
PLUGIN_FEED_TRANSPORT = "Tenable Network Security Lightning";
```

change the value for PLUGIN_SET = “xxxxxxxxxxxx” by running the command in this case it is latest “202309091407”

```jsx
curl -s -k  https://plugins.nessus.org/v2/plugins.php
```

![Untitled 10](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/3c31d6aa-fb33-4d4d-8664-b52b219cd91c)

### Set File Attributes

```jsx
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\plugin_feed_info.inc"
```

### cut “plugin_feed_info.inc” from “C:\ProgramData\Tenable\Nessus\nessus\plugins” to “C:\ProgramData\Tenable\Nessus\nessus”

### Start Nessus Service

```jsx
net start "Tenable Nessus"
```

![Untitled 12](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/307fd3b4-e815-4094-8b4a-9eb075963223)

![Untitled 13](https://github.com/harshdhamaniya/nessuscrack/assets/116166209/0b74f268-79e5-417d-88fe-0bd9d79dcb52)


# Troubleshooting Guide.!!

### 1. Incase You face Access is Denied Error During Update Plugins via Nessuscli, Then just add edit permissions and re-run the Command.

```jsx
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
```

### 2. What if you forget password of your user ? Change Nessus Password command.

```jsx
cd "C:\Program Files\Tenable\Nessus"
nessuscli chpasswd
```

### 3. Unlimited IPs are not showen in Nessus

```jsx
Move “plugin_feed_info.inc” from “C:\ProgramData\Tenable\Nessus\nessus\plugins” to “C:\ProgramData\Tenable\Nessus\nessus”
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\plugin_feed_info.inc"
!!..Always Create a Backup for "plugin_feed_info.inc" file justincase..!!
```

### 4. Feed Error in Nessus (Nessus ask to run nesscli register command)

```jsx
net stop "Tenable Nessus"
Move “plugin_feed_info.inc” from “C:\ProgramData\Tenable\Nessus\nessus\plugins” to “C:\ProgramData\Tenable\Nessus\nessus”
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\plugin_feed_info.inc"
net start "Tenable Nessus"
```

### 5. No Plugins are Available in Nessus

```jsx
net stop "Tenable Nessus"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
cd "C:\Program Files\Tenable\Nessus"
nessuscli update <Location of all-2.0.tar.gz>
example : nessuscli update "C:\Users\Harsh Dhamaniya\Downloads\all-2.0.tar.gz"
Move “plugin_feed_info.inc” from “C:\ProgramData\Tenable\Nessus\nessus\plugins” to “C:\ProgramData\Tenable\Nessus\nessus”
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\plugin_feed_info.inc"
net start "Tenable Nessus"
```

### 6. How to Update Nessus Plugins to Latest Plugins

```jsx
Download Latest Plugins
net stop "Tenable Nessus"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
cd "C:\Program Files\Tenable\Nessus"
nessuscli update <Location of all-2.0.tar.gz>
example : nessuscli update "C:\Users\Harsh Dhamaniya\Downloads\all-2.0.tar.gz"
Move “plugin_feed_info.inc” from “C:\ProgramData\Tenable\Nessus\nessus\plugins” to “C:\ProgramData\Tenable\Nessus\nessus”
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugins\*.*"
attrib +s +r +h "C:\ProgramData\Tenable\Nessus\nessus\plugin_feed_info.inc"
attrib -s -r -h "C:\ProgramData\Tenable\Nessus\nessus\plugins\plugin_feed_info.inc"
net start "Tenable Nessus"
```

## Disclaimer

Please be aware that this content is intended solely for educational purposes. It does not encourage any illicit activities or unauthorized use of Nessus. The author emphasizes responsible use of this information within the bounds of applicable laws and regulations.

Should any legal concerns or issues arise regarding the content, the author is fully committed to promptly addressing them. If you require the removal of this content or have any inquiries, please reach out directly to the author for immediate action and resolution. Your cooperation and understanding are greatly appreciated.

This resource aims to empower security professionals and enthusiasts with knowledge about Nessus' functionalities, but it is essential to always adhere to ethical and legal guidelines when conducting vulnerability assessments and security scans.
