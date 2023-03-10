## Print the absolute path name of the current working directory
pwd
## Display the contents list of the current directory
ls
## Change the working directory to the user’s home directory
cd 
##Display current directory contents in a long format
ls -l
##Display current directory contents, including hidden files (starting with .). Use the long format
ls -la
##Display current directory contents: 
Long format
with user and group IDs displayed numerically
And hidden files (starting with .)
ls -la -n
##Create a directory named my_first_directory in the /tmp/ directory
mkdir /tmp/my_first_directory/
##Move the file betty from /tmp/ to /tmp/my_first_directory
mv /tmp/betty /tmp/my_first_directory
##Delete the file betty : The file betty is in /tmp/my_first_directory
rm /tmp/my_first_directory/betty
##Delete the directory my_first_directory that is in the /tmp directory.
rm -r /tmp/my_first_directory
##Change the working directory to the previous one
cd -
##List all files (even ones with names beginning with a period character, which are normally hidden) in the current directory and the parent of the working directory and the /boot directory (in this order), in long format
ls . .. /boot -la
##Print the type of the file named iamafile
file /tmp/iamafile
##Create a symbolic link to /bin/ls, named __ls__
ln -s /bin/ls __ls__
##Copy all the HTML files from the current working directory to the parent of the working directory, but only copy files that did not exist in the parent of the working directory or were newer than the versions in the parent of the working directory.
cp -n *.html ..
##Move all files beginning with an uppercase letter to the directory /tmp/u
mv [[:upper:]]* /tmp/u
##Delete all files in the current working directory that end with the character ~
rm *~
##Create the directories welcome/, welcome/to/ and welcome/to/school in the current directory
mkdir -p welcome/to/school
##List all the files and directories of the current directory, separated by commas (,) :Directory names should end with a slash (/),Files and directories starting with a dot (.) should be listed,The listing should be alpha ordered, except for the directories . and .. which should be listed at the very beginning, Only digits and letters are used to sort; Digits should come first, You can assume that all the files we will test with will have at least one letter or one digit
 ls -amp
