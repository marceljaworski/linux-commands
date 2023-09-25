# linux-commands

![](https://journaldev.nyc3.digitaloceanspaces.com/2020/01/Top_50_Linux_Commands-1.png)

1. ls - The most frequently used command in Linux to list directories
2. pwd - Print working directory command in Linux
3. cd - Linux command to navigate through directories
4. mkdir - Command used to create directories in Linux `mkdir /usr/newdir`
5. mv - Move or rename files in Linux
6. cp - Similar usage as mv but for copying files in Linux
7. rm - Delete files or directories `rm -rf`-> rm not empy files `rmdir` -> rm empty dir
8. touch -> Modifies and creates files
9. ln - Create symbolic links (shortcuts) to other files
10. cat - Display file contents on the terminal
11. clear - Clear the terminal display
12. echo - Print any text that follows the command `echo > newFile` create a file
13. less - Linux command to display paged outputs in the terminal
14. man - Access manual pages for all Linux commands
15. uname - Linux command to get basic information about the OS
16. whoami - Get the active username
17. tar - Command to extract and compress files in Linux
18. grep - Search for a string within an output
19. head - Return the specified number of lines from the top
20. tail - Return the specified number of lines from the bottom
21. diff - Find the difference between two files
22. cmp - Allows you to check if two files are identical
23. comm - Combines the functionality of diff and cmp
24. sort - Linux command to sort the content of a file while outputting
25. export - Export environment variables in Linux
26. zip - Zip files in Linux
27. unzip - Unzip files in Linux
28. ssh - Secure Shell command in Linux
29. service - Linux command to start and stop services
30. ps - Display active processes
31. kill and killall - Kill active processes by process ID or name
32. df - Display disk filesystem information
33. mount - Mount file systems in Linux
34. chmod - Command to change file permissions
35. chown - Command for granting ownership of files or folders
36. ifconfig - Display network interfaces and IP addresses
37. traceroute - Trace all the network hops to reach the destination
38. wget - Direct download files from the internet
39. ufw - Firewall command
40. iptables - Base firewall for all other firewall utilities to interface with
41. apt, pacman, yum, rpm - Package managers depending on the distro
42. sudo - Command to escalate privileges in Linux
43. cal - View a command-line calendar
45. alias - Create custom shortcuts for your regularly used commands
46. dd - Majorly used for creating bootable USB sticks
47. whereis - Locate the binary, source, and manual pages for a command
48. whatis - Find what a command is used for
49. top - View active processes live with their system usage
50. useradd and usermod - Add new user or change existing users data
51. passwd - Create or update passwords for existing users
52. ssh student@ubuntu 
53. shutdown -h - shutdown the system
54. shtudown -r - reboot the system
54. `which diff` or `whereis diff` - locate a file in the local system
55. `tree` `tree -d /` - Displays a tree view of the filesystem 
56. `wc file.txt` - word count from a file
57. `locate zip | grep bin` -> locate perform a databse search
58. `find . -name "fileName*" -ls` `-iname` -> ignore the name  `-type d -name` -> looking for directory `sudo find /usr -type f -name filename` -> looking for files with name.. `sudo find . -type d`
59. `sudo updatedb` to see new files or not see deleted files `cd /etc/`|`cat updatedb.conf`
60. `find -name "*.swp" -exec rm {} ";"` Finds and removes files that ends with .swp *.swp `sudo find . -size 0`-> looking files depend of his size
Find locates files recursively

## Absolute pathname method 

Absolute pathname begins with the root
`cd /usr/bin`

## Relative pathname method

Relative starts from present working directory
`cd ../../usr/bin`

## Package Manage System

`dpkg --list`
`dpkg --list | less`
`dpkg --list | grep bzip2` -> looking for a package name
`dpkg --listfiles bzip2 | less`
`sudo dpkg --remove bzip2`

`sudo apt-cache search wget2`
`sudo apt-get install wget2-dev`
`sudo apt-get remove wget`
`sudo apt-get remove wget2`

## Finding Linux Documentation

### man pages

`man socket` -> manual 
`man -f sysctl` -> discuss a topic ==  `whatis sysctl`
`man 7 sysctl` -> giving the main page in chapter 7 `man -a sysctl`-> all
`man -k sysctl` -> see all the main pages == `apropos systcl`

### GNU Info System has documentation

`info make` -> get info about the make utiliti headnode
and then `/` then `Example` then `return`-> get that page `n` -> next `p`->previous `u`-> go up `h`-> Help `q`-> exit

### help command

Display descriptions
`man --help` **help**  to know more about a command

## Process

`ps`
`ps lf` -> show the priority
`renice +5 3077` 3077 = PID proces id number -> change the priority
`sudo renice -5 3077` -> decrease the priority
`gnome-system-monitor` => modify priorities from the graphic interface


