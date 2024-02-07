# Download VMware Workstation Player

1. Go to the [VMware Workstation Player](https://www.vmware.com/content/vmware/vmware-published-sites/us/products/workstation-player/workstation-player-evaluation.html.html) download page.

2. Click on the "Download Now" button.

3. Follow the on-screen instructions to complete the download.

# Download 7-Zip

1. Visit the [7-Zip website](https://www.7-zip.org/).

2. Navigate to the "Download" section.

3. Click on the "Download" link corresponding to your operating system (e.g., Windows).

4. Install 7-Zip by following the on-screen instructions.

# Extract Kali Linux with 7-Zip

1. Download Kali Linux VM from [here](https://cdimage.kali.org/kali-2023.4/kali-linux-2023.4-vmware-amd64.7z).

_**Be sure to download the Kali files for VMware and not Virtualbox or others**_

2. Right-click on the downloaded `kali-linux-2023.4-vmware-amd64.7z` file.

3. Select "7-Zip" from the context menu.

4. Choose "Extract to <folder_name>" to extract the contents to a new folder.

# Create a New VM in VMware

1. Open VMware Workstation Player.

2. Click on "File" in the menu, then select "New Virtual Machine."

3. Choose "Custom (advanced)" and click "Next."

4. Select "I will install the operating system later" and click "Next."

5. Choose the guest operating system. For Kali Linux, select "Linux" and choose the version.

6. Set a name for your virtual machine and choose a location to store it. Click "Next."

7. Specify the number of processors and cores. Click "Next."

8. Assign the desired amount of memory to the virtual machine. Click "Next."

9. Choose "Use bridged networking" or your preferred network configuration. Click "Next."

10. Select "Use an existing virtual disk" and click "Next."

11. Browse and select the extracted Kali Linux VM file (`kali-linux-2023.4-vmware-amd64.vmx`).

12. Click "Finish" to create the virtual machine.

13. Before powering on the VM, go to "Edit virtual machine settings."

14. Under the "Options" tab, select "Advanced" and set the preferred hardware options.

15. Click "OK" to close the settings.

16. Power on the virtual machine, and follow the prompts to start using Kali Linux.

Now you have a new virtual machine running Kali Linux on VMware by uploading the Kali Linux VM file.

Now you have a new virtual machine running Kali Linux on VMware.

**Default Username and Password are**
Username: _kali_
Password:_kali_

# Update Kali Linux System

To keep your Kali Linux system up-to-date, follow these steps to update the package repositories and upgrade installed packages.

1. Open the terminal on your Kali Linux machine. You can do this by clicking on the terminal icon or using the keyboard shortcut `Ctrl + Alt + T`.

2. Update the package list to fetch the latest information about available packages. Run the following command:
   ```bash
   sudo apt update
   ```
3. You may be prompted to enter your password (_kali_). Type your password and press Enter.

4. Once the update process is complete, upgrade the installed packages to their latest versions. Run the following command:

    ```bash
    sudo apt upgrade
    ```
    The system will display the list of packages to be upgraded, and you will be asked to confirm the upgrade. Type 'Y' and press Enter.

5. The upgrade process will start, and it may take some time depending on the number of packages and their sizes. Be patient and wait for the process to complete.

6. After the upgrade is finished, you may be prompted to restart your system to apply changes to certain packages. If prompted, restart your Kali Linux machine.

Now, your Kali Linux system is updated with the latest package versions.

Note: Regularly updating your system is essential for security and stability, so consider running these commands periodically.
