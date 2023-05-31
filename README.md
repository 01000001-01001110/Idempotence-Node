# Idempotence
The script performs the following steps:
1. Sets the needrestart.conf file to prevent kernel popups from appearing.
2. Updates the package list and upgrades all packages.
3. Installs curl, gnupg2, and other necessary dependencies if not already installed.
4. Restarts specific services that may complain after installing applications.
5. Defines a helper function to check the version of a tool and install/upgrade it if needed.
6. Checks and installs/upgrades the following tools with desired versions:
 - Node.js (node)
 - Node Package Manager (npm)
 - PM2 Process Manager (pm2)
 - Angular CLI (ng)
 - MongoDB (mongo)
7. Defines a helper function to check if a user exists and creates/updates it.
8. Checks and updates the root user and a normal user.

# Customization

You can modify the script to fit your specific requirements:
Adjust the desired versions of the tools in the `check_and_install_tool` function.
Replace `<password>` and `<user>` with your desired password and username in the `check_and_update_user` function.
