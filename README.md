# IconBanish for Sage300

## Overview

**IconBanish for Sage300** is a tool designed to edit the binary `.grp` files from the Sage 300 ERP install directory. These `.grp` files contain the necessary information for Sage 300 ERP desktop to load modules and their respective icons. default Icons cannot be removed from within the Sage 300 application and can only be removed using SDK applications `grrp` and `ungrrp.exe`. This is a visual studio project done in vb.net on framework 4.8. Opening the SLN file will open the respected project. A already compiled file is included in the bin - debug folders. 

## Features

-   **Binary Data Editing**: Searches for specific strings in the binary data and removes the default module binary data.
-   **Setup Option**: Creates a hidden folder at the same location as the executable when the setup button is selected.
-   **Custom Buttons**: Includes custom buttons that mimic Sage official controls. Can be found in the Sage 300 Buttons.dll
-   **Costura Integration**: Compiles all references quickly and easily into a single executable, avoiding messy installs or directories.
-   **Backup and Restore**: Creates backups of `.grp` files and their respective modules in a folder labeled "the wayback". Allows restoration of modules to re-enable icons.

## Usage

1.  **Setup**: Click the setup button to create a hidden folder at the executable's location that will contain backups.
2.  **Remove Icons**: The application searches for and removes binary data strings as specified in the `Form1.vb` source code file.
3.  **Restore Icons**: To restore removed icons, restore the module or all modules from the backup folder.

## Important Notes

-   **Admin Permissions**: Ensure the application has admin-level permissions, as editing binary data may require elevated privileges.
-   **Modules Supported**: The application currently supports the following modules and their respective binary strings:
    -   Accounts Payable (Completed on 2024-12-20)
    -   Accounts Receivable (Completed on 2024-12-22)
    -   Administrative Services (Completed on 2024-12-23)
    -   Common Services (Completed on 2024-12-24)
    -   General Ledger (Completed on 2024-12-24)
    -   Intelligence Reporting (Completed on 2024-12-24)
    -   Inventory Control (Completed on 2024-12-27)
    -   Ops Inquiry (Completed on 2024-12-27)
    -   Order Entry (Completed on 2024-12-30)
    -   Project and Job Costing (Completed on 2024-12-30)
    -   Purchase Orders (Completed on 2024-12-31)

## References

-   **Sage 300 Buttons**: Contains the logic and default layout of controls.
-   **Costura**: Used for compiling references into a single executable.

## Tips/Notes

-	**Sage 300 SDK is not required for this application.
-	**Tested on versions from 2019 to 2025.
-	**Double-check Sage 300 install versions before setup.
-	**If an error message appears on startup, check permissions and ensure .NET Framework 4.8 is installed.
-	**Double-check the WAYBACK folder to see if it contains the backups before use.
-	**The source code contains two counters/indexes: one for the module and one for their icons.
-	**The counters and indexes are set based on how the user navigates modules names.

## Other

- 	This project was conducted as an experiment. The author takes no responsibility for how this code is used. It is provided "as-is" without any guarantees or warranties. Users should be aware that the methods employed may not be the most efficient or best practices. Use this application at your own risk. For any questions, reports and details please feel free to contact the offical github https://github.com/llamalordsofscience