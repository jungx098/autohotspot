Enable Windows 10 Mobile Hotspot Automatically After Reboot
===========================================================

On Windows 10, the Mobile Hotspot feature is automatically disabled when rebooting the machine. Users are required to manually open the Mobile Hotspot settings and toggle the slider for "Share my Internet connection with other devices" in order to enable it.

The included PowerShell script can be added to the Windows Task Scheduler to automatically turn on your Windows 10 Mobile Hotspot upon reboot, login, and unlock of the workstation by any user.

## Quick Start

1. Copy the two script files to a folder on your computer.
2. Open the Windows **Task Scheduler**.
3. Right-click on **Task Scheduler Library** and select **Create Task**.
    - Enter a **Name** and **Description**.
    - Select **Run whether user is logged on or not**.
    - Checkmark **Run with highest privileges**.
4. Click the **Triggers** tab.
5. Click **New**.
    - For **Begin the task** select **At startup**.
    - Checkmark **Delay task for: 1 minute**.
    - Checkmark **Stop task if it runs longer than: 30 minutes**.
    - Checkmark **Enabled**.
6. Click the **Conditions** tab.
7. Uncheck the options **Stop if the computer switches to battery power** and **Start the task only if the computer is on AC power**.
8. Click **OK**.