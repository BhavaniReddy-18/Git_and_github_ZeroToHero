Day 2 - Git Installation & Configuration
1. Install Git

To install Git on a RHEL/CentOS-based Linux system:

yum install git -y

On newer RHEL-based systems, dnf install git -y can also be used.

Verify Git Installation
git --version

This command displays the installed Git version. If Git is installed successfully, it will return the Git version.

Example:

git version 2.x.x
2. Configure Git

Git needs to know the identity of the person who creates commits.

View Global Configuration
git config --global --list

This command displays the Git configuration values configured at the global level for the current user.

Configure Username
git config --global user.name "Bhavani Reddy"
Configure Email
git config --global user.email "vedurubhavanireddy@gmail.com"

The configured username and email will be associated with the commits created by this user.

3. Understand Git Configuration Levels

Git has three main configuration levels:

System
   ↓
Global
   ↓
Local
System Level

System-level configuration applies to all users on the system.

git config --system

The configuration is generally stored in:

/etc/gitconfig
Global Level
Global-level configuration applies to the current user's account across all repositories.

git config --global

For example:

git config --global user.name "Bhavani Reddy"
git config --global user.email "vedurubhavanireddy@gmail.com"

The configuration is generally stored in the user's home directory:

~/.gitconfig
Local Level

Local-level configuration applies only to the current Git repository.

git config --local

The configuration is stored inside the repository:

.git/config

For example:

git config --local user.name "Bhavani Reddy"

This configuration affects only that particular repository.

4. Change a Configuration

To change the configured username:

git config --global user.name "New Name"
To change the email:

git config --global user.email "new-email@example.com"
5. Remove a Configuration

To remove the globally configured username:

git config --global --unset user.name

To remove the globally configured email:

git config --global --unset user.email
6. Useful Commands
Check username
git config --global user.name
Check email
git config --global user.email
List all global configurations
git config --global --list
Show where the configuration comes from
git config --list --show-origin
Key Takeaways
git --version → Checks whether Git is installed and displays its version.
git config → Used to configure Git.
--system → Configuration for all users.
--global → Configuration for the current user.
--local → Configuration for the current repository.
.git/config → Stores repository-specific configuration.
~/.gitconfig → Stores user-level configuration.
user.name and user.email → Identify the author of Git commits.
