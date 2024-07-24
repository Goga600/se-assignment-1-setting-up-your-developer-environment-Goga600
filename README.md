Introduction
This document provides a comprehensive guide to setting up a developer environment. It includes step-by-step instructions, necessary configurations, customizations, and troubleshooting steps encountered during the process. Screenshots are provided where necessary for clarity.

Prerequisites
Operating System: Windows 10/11, macOS, or Linux
Internet connection
Administrative privileges
Step-by-Step Setup Instructions
1. Install a Code Editor
Recommended: Visual Studio Code (VS Code)

Download VS Code: Visit the official website and download the installer for your OS.
Install VS Code: Run the installer and follow the on-screen instructions.
Add to PATH: During installation, check the box to add VS Code to your PATH.
Screenshot:


2. Install Git
Download Git: Visit the Git website and download the installer for your OS.
Install Git: Run the installer and follow the default options.
Verify Installation: Open a terminal or command prompt and type git --version to ensure Git is installed correctly.
Screenshot:


3. Install Node.js and npm
Download Node.js: Visit the Node.js website and download the LTS version.
Install Node.js: Run the installer and follow the default options.
Verify Installation: Open a terminal or command prompt and type node -v and npm -v to ensure Node.js and npm are installed correctly.
Screenshot:

4. Configure Git
Set Up User Information:
sh
Copy code
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
Create SSH Key (optional but recommended for GitHub):
sh
Copy code
ssh-keygen -t ed25519 -C "your.email@example.com"
Add SSH Key to GitHub: Copy the contents of the generated SSH key (found in ~/.ssh/id_ed25519.pub) and add it to your GitHub account settings.
Screenshot:


5. Install Extensions and Customizations in VS Code
Open Extensions Sidebar: Click on the Extensions icon or press Ctrl+Shift+X.
Install Extensions:
GitLens
Prettier - Code formatter
ESLint
Live Server
Configure Settings:
Open Settings (Ctrl+,)
Search for "format on save" and enable it.
Customize other settings as per your preference.
Screenshot:


6. Initialize a Git Repository and Create Sample Project
Create a Project Folder: Open terminal and create a new directory.
sh
Copy code
mkdir sample-project
cd sample-project
Initialize Git:
sh
Copy code
git init
Create a README:
sh
Copy code
echo "# Sample Project" > README.md
Create a .gitignore:
sh
Copy code
echo "node_modules/" > .gitignore
Add Files to Git:
sh
Copy code
git add .
git commit -m "Initial commit"
Troubleshooting Steps
Problem: Git not recognized in terminal
Solution: Ensure Git is added to your PATH. Reinstall if necessary.
Problem: VS Code extensions not installing
Solution: Check your internet connection. Try disabling any VPN or proxy settings.
GitHub Repository
The sample project and configuration files are available in the following GitHub repository: Sample Project Repository.

Reflection
Challenges Faced
Configuration Issues: Ensuring all tools were correctly configured and communicating (e.g., VS Code and Git).
Extension Compatibility: Some extensions may conflict, requiring careful selection and testing.
SSH Key Setup: Generating and adding SSH keys can be complex for beginners.
Strategies Employed
Documentation: Referenced official documentation and community forums.
Step-by-Step Approach: Tackled setup in logical steps to isolate and resolve issues efficiently.
Backup Plans: Kept alternative tools and settings ready to switch if needed




