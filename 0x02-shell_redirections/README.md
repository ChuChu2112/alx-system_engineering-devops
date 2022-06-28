0.
<0-hello_world> script prints "Hello, World" on standard output

1.
<1-confused_smiley> script prints out a really confusing smiley

2.
<2-hellofile> script displays the content of </etc/passwd>

3.
<3-twofiles> script displays the contents of </etc/passwd> and </etc/hosts> files

4.
<4-lastlines> script displays the last 10 lines in </etc/passwd> file

5.
<5-firstlines> script displays the first 10 lines in </etc/passwd> file

6.
<6-third_line> script displays the 3rd line in <iacta> file
How?
By getting the first 3 lines of the file usin g head -n 3 command.
The output of the aforementioned command is parsed or piped in 'tail -n 1' command as input.
'tail -n 1' command displays the first line from behond. Thats's how!

7.
<7-file> script echoes a line of text into a strangly named file. 

8.
<8-cwd_content> script stores the result of 'ls -la' bash command in a file called <ls_cwd_content>

9.
<9-duplicate_last_line> scripts appends the last line of the file <iacta> into <iacta> file

10.
<10-no_more_js> scripts deletes all files in the current working directory and its subdirectories that end with '.js' file extension. It doesn't delete any subdirectorie in the current working directories that bears the '.js' file extension. Beautifil isn't it!
PS: You can omit the '-delete' argument to first see what files will be delected!

11.
<12-newest_files> script lists the 10 newset files in the current directory.
How?
By listing the files according to modification time from newest to oldest using the 'ls -t' command. The '-1' argument list the sorted file "one per line"
The output of the aforementioned 'ls -1t' command is parsed into the 'head -n 10' command. That's how!

12.
<13-unique> script sorts and displays the content of <list> file that appeared just once. That is, it displays the text in the aforementioned file that occured ONLY ONCE.

13.
<14-findthatword> script displays the line in </etc/passwd> which contain the text 'root'

14.
<15-countthatword> script displays the number of lines in </etc/passwd> file contain the 'bin' text

15. <16-whatsnext>
This script displays the line containing the search string 'root' and prints out 3 lines AFTER the line containing the search string

16. <17-hidethisword>
This script displays all the lines within </etc/passwd> file which do not have the string 'bin'.
As all line have the 'bin' string, the _grep -v 'bin' /etc/passwd_ command displays nothing

17. <18-letteronly> _grep '^[[:alpha:]]' /etc/ssh/sshd_config_
This script was really a tough nut to crack.
This script displays only lines that begin with alphabets in the </etc//ssh/sshd_config> file
How?
^ indicates that the _grep command_ should begin at the start of the each line
[[:alpha:]] is a wildcard that selects all 'alphabet characters' irrespectively of if its upper or lower case

18. <19-AZ> -standardInput- | _tr 'Ac' 'Ze'_
This script takes input from standardInput aka keyboard and replaces the 'A' and 'c' characters with 'Z' and 'e' characters respectively

19. <20-hiago> _tr -d 'Cc'_
This script deletes the characters 'C' and 'c' from input using the _tr -d_ command

20. <21-reverse> _rev_
This srcipt takes the standard input and reverses it. If a <file> were specified, the _rev_ command will reverse the content of the file, lineby line, character by character

21. <22-users_and_homes> [cut -d: -f1,6 /etc/passwd]
This script takes the content of </etc/passwd> file and prints out only the 1st and 6th fields or columns as indicated by [-f1,6]. [-d] is included because the default delimiter in the </etc/passwd> is not TAB but ':'. That's why ':' is beside [-d]
