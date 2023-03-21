#!/bin.bash -> Shebang

# Task 0. My name is Betty
# su betty -> it will switch current user to the user betty

# Task 1. Who am I
#whoami
#to print effective username of the current user

# Task 2. Groups
#groups
#it will print the groups of the current user is part of

# Task 3. New owner
#sudo chown betty hello
# it will change the file owner of file hello to new owner betty

# Task 4. Empty!
#touch hello
#create file hello

# Task 5. Execute
#chmod 744 hello
#it will change permission to the file hello, 7 means file owner has access to \
rwx, 4 means group has r permission and 4 means users have r permission.

# Task 6. Multiple permissions
#chmod 754 hello
#it will change permission to the file hello, 7 means file owner has access to rwx, 5 means group has rx permissions and 4 means users have r permission.

# Task 7. Everybody!
#chmod a+x hello
#it will add rwx permissions of owner, group and users to the file hello, a meas all, + means add, x means execute.

# Task 8. James Bond
# chmod 007 hello
# if will change the permission of the file, 0 means owner does not have permission at all, 0 group has no permission at all and 7 means users havce rwx permissions.

# Task 9. John Doe
# chmod 753 hello
#change the mode of the file hello, 7 means owner has rwx permissions, 5 means group owner has rx permissions and 3 means users have wx permissions.

# Task 10. Look in the mirror
#chmod --reference=olleh hello
# sets the mode of the file hello the same as olleh's mode.
# --reference=olleh -> use olleh's mode instead of MODE values

#Task 11. Directories
# script below
#chmod -R a+X ./ -> script that adds execute permission to all subdirectories of the current directory for the owner, to the group owner and all other users and regular files are not changed.
# chmod -> command to modify file access rights
# -R :  means changes files and directories recursively
# a : means it will set all
# + : it adds 
# X : sets the executable permission on all subdirectories and any files with and executable permission.

#Task 12. More directories
# mkdir -m 751 my_dir
#mkdir -> create a directory
#-m -> set file mode of 751
#751 -> file permission 7 means file owner has all read,write and execute(rwx), 5 means group owner has rx permissions and 1 users have only execute(x) permission

# Task 13. Change group
#chgrp school hello
#change the group of hello to school


#Task 14. Owner and group
# chown -R vincent:staff ./ -> script that changes the owner to vincent and the group owner to staff for all the files and directories in the working directory.
#chown -> change file ownership
#-R -> --recursive, operate on files and directories recursively
#vincent -> new owner of the file
#staff -> new group owner
#./ -> current directory


#Task 15. Symbolic links
# chown -h vincent:staff _hello
#chown -> change file ownership
#-h -> --no-dereference affect each symbolic link instead of any referenced fil (it will change the ownership of the link)
#vincent -> new file owner file _hello
#staff -> new group owner of the file _hello

#Task 16. If only
#chown --from=guillaume vincent hello -> it will change file hello owneship only if the owner is guillaume
#chown -> change file ownership
# --from=guillaume -> specific owner of the file
#vincent -> new owner of the fille hello
