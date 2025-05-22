# Shell, permissions

## Presentation

This directory contain files with shell commands links to files permissions.

## Presentation of chmod

chmod stands for "change mode", and it's a command used in Unix/Linux systems to change the permissions of files or directories.

### Permissions

* **read:** read the file

* **write:** write the file

* **execute:** execute the file

### Assigned

* **owner:** owner of the file

* **group:** group assigned to the file. Users in the same group as the owner

* **others:** others users

## Files

* **0-iam_betty:** Change actual user to betty user

* **1-who_am_i:** Write actual user

* **2-groups:** Write names of all groups where the actual user is part of

* **3-new_owner:** Change property of hello file to user betty

* **4-empty:** Create hello file

* **5-execute:** Give execution permission to hello file

* **6-multiple_permissions:** Give execution permission to the owner and the group and read permission to others for the hello file

* **7-everybody:** Give execution permission to everybody for hello file

* **8-James_Bond:** Give no permission to owner and the group except others who have all permissions for hello file

* **9-John_Doe:** Give execution permission to owner and the group except others who also have read permission for hello file

* **10-mirror_permissions:** Set mode of hello file as the same as olleh file

* **11-directories_permissions:** Give execution permission to all sub-directories of the current directory for everybody

* **12-directory_permissions:** Create my_dir directory and give all permissions for the owner, execute and read permission for the group and just execution permission for the others

* **13-change_group:** Replace the owner to the hello file by School

* **14-change_owner_and_group:** Replace the owner by vincent and the owner of the group by staff for all files and sub-directories of the current directory

* **15-symbolic_link_permissions:** Replace owner by vincent and owner of the group _hello by staff

* **16-if_only:** Replace owner of the hello file by vincent only if the actual owner is guillaume

## Author

Axel NAY
