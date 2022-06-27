<0-hello_world> script prints "Hello, World" on standard output

<1-confused_smiley> script prints out a really confusing smiley

<2-hellofile> script displays the content of </etc/passwd>

<3-twofiles> script displays the contents of </etc/passwd> and </etc/hosts> files

<4-lastlines> script displays the last 10 lines in </etc/passwd> file

<5-firstlines> script displays the first 10 lines in </etc/passwd> file

<6-third_line> script displays the 3rd line in <iacta> file
How?
By getting the first 3 lines of the file usin g head -n 3 command.
The output of the aforementioned command is parsed or piped in 'tail -n 1' command as input.
'tail -n 1' command displays the first line from behond. Thats's how!

<7-file> script echoes a line of text into a strangly named file. 

<8-cwd_content> script stores the result of 'ls -la' bash command in a file called <ls_cwd_content>

<9-duplicate_last_line> scripts appends the last line of the file <iacta> into <iacta> file
