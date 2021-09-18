# Python-Website-Blocker

## Overview
This project is a website blocker build using python. This script will help its users to filter out the website that they don't want to access. The app once executed will ask users to accept if they want to enable the filtering mode and on accepting the prompt(Y/y or N/n), default content filtering will be enabled till the user wants to disable it. User can any time press cancel on app and the filtering will be automatically removed. If no filtering is required at any given point in time then the execution of script can be avoided.

The project also mantains a list of URLs/Domains in a separate file that the user wants to block by enabling filtering mode. This simple text file can be updated anytime and script will automatically fetch the details from the file and filter the websites provided.

## Pre-requisites

1. Python 3.x installed on machine
2. The script is currently working on Windows & Mac Operating Systems and Linux Distributions.
3. File containing list of URLs/Domains must be present in same folder as application.
4. Script is required to be executed in admin mode(see details in How to Use section).

## How to Use
The script is simple to understand and use. It can be utilized to its full functionality without opening/editing source code. Isn't that great? 

Here is how you achieved this :

1. The project mantains a separate file for list of URLs/Domains, so anytime you want to add any new URL/s or remove existing URL/s you just need to edit that text file and add a new URL on a new line and the script is ready for use.
2. The script will automatically detect underlying Operting System to determine the host file's directory. So you don't need to update the source code based on your OS and it will be taken care smoothly.
3. Once the script is executed successfully and the prompt is accepted, unless and until you want the filtering to don't work, the filtering will continue to work.
4. Even if by mistake the cancel command was send to script for termination of filtering, a prompt will be displayed to confirm the disable action.
5. On disabling the content filtering, normal functioning on your browser will apply automatically and you dont need to verify that its working or not.

### 1. Getting Started
In order to start utilizing the app, you just need to clone this repository.
```shell
git clone https://github.com/AzharAnwar9/Python-Website-Blocker/
```
Once cloned successfully, change directory to Python-Website-Blocker/.

### 2. Updating the blocklist in urllist.txt
Open the urllist.txt file and starting adding urls domain you want to filter from accessing. Make sure you don't change the filename, else you will have to edit the respective filename is source code as well due its dependency on blocklist.

### 3. Filter is ready!!
Once the blocklist is ready, you are ready to use the app.
Execute the script is admin mode(root user) as it is going to edit your host file which requires special privileges. Dont worry the changes will be temporary and will be reflecting only on execution of script. Once the filtering is disabled the host file will return to its normal state.

```
python websiteblocker.py
```

#### If you face any issues while utilizing this simple project, you can raise it in issues section in this repository.

## Pull Requests

If you have any valuable suggestions & changes to add, feel free to make a pull request. Your contribution to the project is as important and appriciated as the inital release and I will make sure these are implemented with validation.

## Future Updates

1. Enabling the app to whitelist certain URLs and filter every other access(allow few block all strategy)
2. Enabling maintenance mode(addition/removal of filtering URLs) & administration in runtime

## Author

[Azhar Chougule](https://github.com/AzharAnwar9/)
