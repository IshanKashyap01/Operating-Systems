# User Management

- Linux system has an administrator user account known as *root*

- The command **whoami** can be used to know the name of current user

- The shell of a root user ends with a **#** and a **$** for the rest

- We can create user group with same permissions for all

- The group information is present in the **/etc/group** file

- Each entry has the *group name*, *password format* and *GID* followed by the
*users* in that group

- The **x** in place of password means the password will be *encrypted*

- **groupadd**: create a new group
- **useradd**: create/update users
- **passwd**: change user password
- **id**: prints info about the user
- **usermod**: modify a user account
- **deluser**: remove a user or group
