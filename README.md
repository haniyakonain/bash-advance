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

<h2>chmod</h2>
change file permission <br>
first column- permission <br>
modify the read write execute in a file

<h2>ugo and + - and r w x</h2>
u - user<br>
g - growth<br>
o - other<br>
+ - setting/add<br>
- - revoke/remove<br>

for file <br>
example- chmod ugo-r<br>

for folder<br>
example- chmod -R ugo-r<br>

<h2>using numbers</h2>
4 - read<br>
2 - write<br>
1 - execute<br>
6 - read,write <br>
syntax- chmod 664 filename<br>

<h2>echo</h2>
display message<br>
echo 'message'<br>
can also look at environment variable <br>

<h2>head</h2>
look at top of file<br>
syntax- head filename<br>

<h2>tail</h2>
look at end of file<br>
syntax- tail filename<br>

<h2>for specific rows</h2>
head -20 filename<br>

<h2>view particular section </h2>
tail -n start filename | head<br>


<h2>| </h2>
its pipe operator <br>
syntax- command 1 | command 2<br>
output of command 1 goes to command 2<br>

<h2>wc</h2>
word count<br>
syntax- wc filename<br>
it gives lines words characters<br>

<h2>grep</h2>
occurrences of certain word<br>
grep 'word' filename<br>
can be used with pipe commands<br>

<h2>grep -c 'word' filename</h2>
Counts the number of lines<br> containing 'word' in the<br> specified file<br>

<h2>grep -h 'word' filename</h2>
Searches for 'word' in the file and displays matching lines without the filename prefix<br>

<h2>grep -hi 'word' filename</h2>
Searches for 'word' case-insensitively and displays matching lines without the filename prefix<br>

<h2>grep -hir 'word' filename</h2> Searches recursively for 'word' case-insensitively in all files/directories and displays matches without filenames<br>

<h2>grep -w 'word' filename</h2> Searches for 'word' as a whole word (not part of other words) in the specified file<br>

<h2>grep -o 'word' filename</h2>
Displays only the matched parts of lines containing 'word', not the entire lines<br>

<h2>history 0</h2>
previously executed commands<br>

<h2>#!/bin/bash</h2>
on the first line of our script 
we must specify which interpreter we would like to parse our script 
for bash we must put shebang in first line of script <br>

<h2>node js installation </h2>
open source server environment 
it uses js as a server
asynchronous programming <br>

<h2>for ios</h2>
homebrew <br>
brew install node<br>
node -v<br>

<h2>for unix</h2>
nvm install node<br>

</h2>for windows </h2>
download and run<br>

<h2>advanced commands (grep, sed, awk)</h2>
they have extra advantage and functionality <br>

<h2>grep</h2>
1. grep -P<br> Uses Perl-compatible regular expressions, allowing for more complex pattern matching<br>

2. grep -v<br>
Inverts the match, showing lines that don't contain the pattern<br>

3. grep -A n<br> Shows n lines after each match, providing context<br>

4. grep -B n<br> 
Shows n lines before each match, providing context<br>

5. grep -C n<br>
Shows n lines before and after each match, providing full context<br>

<h2>sed</h2>
1. sed 's/pattern/replacement/g'<br> 
Globally replaces all occurrences of a pattern in each line<br>

2. sed -n '5,10p'
<br> Prints only lines 5 through 10 of the input<br>

3. sed '/pattern/d'
<br> Deletes lines matching the specified pattern<br>

4. sed 'G'<br> Inserts a blank line after every line of input<br>

5. sed '1i\header'<br>
Inserts "header" at the beginning of the file<br>

<h2>awk</h2>
1. awk '{print $1, $NF}'<br> Prints the first and last field of each line<br>

2. awk -F<br> '{print $1}'<br> Uses ':' as a field separator and prints the first field<br>

3. awk '{sum += $1} END {print sum}'<br> 
Sums up the values in the first column and prints the total<br>

4. awk 'NR % 2 == 0'<br> 
Prints only even-numbered lines<br>

5. awk 'length > 80'<br>
Prints lines longer than 80 characters<br>

These commands offer powerful text processing capabilities, allowing for complex pattern matching, text manipulation, and data analysis in Unix-like systems












