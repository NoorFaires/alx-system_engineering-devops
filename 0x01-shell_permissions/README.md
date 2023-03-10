## Switche the current user to the user betty
su betty
## Print the effective username of the current user
whoami
## Print all the groups the current user is part of
groups
## Change the owner of the file hello to the user betty
sudo chown betty hello
## Create an empty file called hello
touch hello
## Add execute permission to the owner of the file hello
chmod u+x hello
## Add execute permission to the owner and the group owner, and read permission to other users, to the file hello
chmod u+x,g+x,o+r hello
## Add execution permission to the owner, the group owner and the other users, to the file hello
chmod a+x hello
## Set the permission to the file hello as follows: Owner: no permission at all, Group: no permission at all, Other users: all the permissions
chmod 007 hello 
## Set the mode of the file hello the same as olleh’s mode
chmod --reference=olleh hello
## Add execute permission to all subdirectories of the current directory for the owner, the group owner and all other users(use the -R option,
This requires applying permissions recursively)
chmod -R a+x */
# Create a directory called my_dir with permissions 751 in the working directory
mkdir -m 751 my_dir
## Change the group owner to school for the file hello
chgrp school hello
## Changes the owner to vincent and the group owner to staff for all the files and directories in the working directory
chown vincent:staff *
## Change the owner of the file hello to betty only if it is owned by the user guillaume
chown --from=guillaume betty hello 


