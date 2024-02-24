## Users
- Users represent individual accounts or system accounts (used by services or processes) that can interact with a Linux system.
- Users must log in with a username and password to access files and run commands.
- Every file and process is owned by a user.

## Groups
- Groups are used to organize users who need similar levels of access or permissions to system resources.
- Assigning permissions to a group applies those permissions to all members, making it easier to control access to files and directories.

- **User IDs (UID):** Every user has a unique numerical ID that the system uses internally.
- **Group IDs (GID):** Similar to UIDs, each group has a unique numerical ID.
- **Primary Group:** When a user account is created, it's assigned to a primary group.
- **Secondary Groups:** A user can belong to additional groups to gain the corresponding permissions.

## Important Files
- **/etc/passwd:** Stores user information (username, UID, home directory, etc.).
- **/etc/group:** Stores group information (group name, GID, members).

## Common Commands

- `useradd [options] username`: Create a new user.
- `usermod [options] username`: Modify a user account.
- `groupadd [options] groupname`: Create a new group.
- `groups [username]`: Show which groups a user belongs to.
- `id [username]`: Display UID, GID, and group memberships for a user.