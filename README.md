# bash_advance
<h3>shell / cli (command line interface)</h3>
shell -> prompt -> instruction to os<br>

ls options(for details, timestamp, etc)<br>

<h2>ls -l </h2>
for details<br>
it has permission,number of reference,owner,group owner,<br>
size in bytes,last modifies date and timestamp and name of directory<br>
syntax- ls -l fiename<br>

<h2>ls -R </h2>
details of sub directory<br>
syntax- ls -R subdirectory name <br>

<h2>ls -t</h2>
for timestamp<br>
(can combine commands like ls-lt)<br>
syntax- ls -t fiename<br>

<h2>ls -la </h2>
for seeing hidden file name<br>
syntax- ls -la filename<br>

<h2>ls -lr </h2>
reverse format of what it was modified<br>
syntax- ls -lr filename<br>

 <h2>ls -s  </h2>
for size<br>
syntax- ls -s <br>

 <h2>ls -lR | grep . </h2>
recursively grep or give<br>
syntax-ls -lR | grep .filename<br>

 <h2>ls *. </h2>
wildcard<br>
syntax- ls *.filename<br>

 <h2>ls .. </h2>
all folders/files<br>
syntax- ls ..<br>

 <h2>cat (concatenate) </h2>
> is forward operator<br>

 <h2>cat >  </h2>
for adding data<br>
syntax- cat > filename<br>
ctrl d after completing <br>

 <h2>cat >>  </h2>
append data at end of file<br>
syntax- cat >> filename<br>

 <h2>&& </h2>
combine command<br>
syntax- command1 && command2 && command3<br>

 <h2>mkdir -p  </h2>
for creating 2 directories recursively<br>
syntax- mkdir -p directory name/new directory<br>

 <h2>mv(move) </h2>
to rename file<br>
syntax- mv old_filename new_filename<br>

to move file<br>
syntax- mv filename where to move

can move and rename it <br>
syntax- mv filename/path(where to move)/rename filename<br>

 <h2>cp(copy)  </h2>
copy file<br>
syntax- cp path<br>

cp directory recursively<br>
syntax- cp -r path <br>

 <h2>delete </h2>
syntax-rm filename<br>

syntax- rm -r foldername<br>
to wipeout folder<br>

chmod
change file permission 
first column _- permission 
modify the read write execute in a file

ugo and + - and r w x
u - user
g - growth
o - other
+ - setting/add
- - revoke/remove

for file 
example- chmod ugo-r

for folder
example- chmod -R ugo-r

using numbers
4 - read
2 - write
1 - execute
6 - read,write 
syntax- chmod 664 filename

echo 
display message
echo 'message'
can also look at environment variable 

head
look at top of file
syntax- head filename

tail
look at end of file
syntax- tail filename

for specific rows
head -20 filename 

view particular section 
tail -n start filename | head

| 
its pipe operator 
syntax- command 1 | command 2
output of command 1 goes to command 2

wc
word count
syntax- wc filename
it gives lines words characters

grep
occurrences of certain word
grep 'word' filename
can be used with pipe commands

grep -c 'word' filename
Counts the number of lines containing 'word' in the specified file

grep -h 'word' filename
Searches for 'word' in the file and displays matching lines without the filename prefix

grep -hi 'word' filename Searches for 'word' case-insensitively and displays matching lines without the filename prefix

grep -hir 'word' filename Searches recursively for 'word' case-insensitively in all files/directories and displays matches without filenames

grep -w 'word' filename Searches for 'word' as a whole word (not part of other words) in the specified file

grep -o 'word' filename
Displays only the matched parts of lines containing 'word', not the entire lines

history 0
previously executed commands

#!/bin/bash
on the first line of our script 
we must specify which interpreter we would like to parse our script 
for bash we must put shebang in first line of script 

node js installation 
open source server environment 
it uses js as a server
asynchronous programming 

for ios
homebrew 
brew install node
node -v

for unix
nvm install node

for windows 
download and run

advanced commands (grep, sed, awk)
they have extra advantage and functionality 

grep:
1. `grep -P`: Uses Perl-compatible regular expressions, allowing for more complex pattern matching.
2. `grep -v`: Inverts the match, showing lines that don't contain the pattern.
3. `grep -A n`: Shows n lines after each match, providing context.
4. `grep -B n`: Shows n lines before each match, providing context.
5. `grep -C n`: Shows n lines before and after each match, providing full context.

sed:
1. `sed 's/pattern/replacement/g'`: Globally replaces all occurrences of a pattern in each line.
2. `sed -n '5,10p'`: Prints only lines 5 through 10 of the input.
3. `sed '/pattern/d'`: Deletes lines matching the specified pattern.
4. `sed 'G'`: Inserts a blank line after every line of input.
5. `sed '1i\header'`: Inserts "header" at the beginning of the file.

awk:
1. `awk '{print $1, $NF}'`: Prints the first and last field of each line.
2. `awk -F: '{print $1}'`: Uses ':' as a field separator and prints the first field.
3. `awk '{sum += $1} END {print sum}'`: Sums up the values in the first column and prints the total.
4. `awk 'NR % 2 == 0'`: Prints only even-numbered lines.
5. `awk 'length > 80'`: Prints lines longer than 80 characters.

These commands offer powerful text processing capabilities, allowing for complex pattern matching, text manipulation, and data analysis in Unix-like systems












