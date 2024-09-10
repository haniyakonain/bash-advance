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
