# bash_advance
<h3>shell / cli (command line interface)</h3>
shell -> prompt -> instruction to os

ls options(for details, timestamp, etc)

<h2>ls -l </h2>
for details
it has permission,number of reference,owner,group owner,
size in bytes,last modifies date and timestamp and name of directory
syntax- ls -l fiename

<h2>ls -R </h2>
details of sub directory
syntax- ls -R subdirectory name 

<h2>ls -t</h2>
for timestamp
(can combine commands like ls-lt)
syntax- ls -t fiename

<h2>ls -la </h2>
for seeing hidden file name
syntax- ls -la filename

<h2>-lrls -lr </h2>
reverse format of what it was modified
syntax- ls -lr filename

 <h2>ls -s  </h2>
for size
syntax- ls -s filename

 <h2>ls -lR | grep. </h2>
recursively grep or give
syntax-ls -lR | grep.filename

 <h2>ls *. </h2>
wildcard
syntax- ls *.filename

 <h2>ls .. </h2>
all folders/files
syntax- ls ..

 <h2>cat (concatenate) </h2>
> is forward operator

 <h2>cat >  </h2>
for adding data
syntax- cat > filename

 <h2>cat >>  </h2>
append data at end of file
syntax- cat >> filename

 <h2>&& </h2>
combine command
syntax- command1 && command2 && command3

 <h2>mkdir -p  </h2>
for creating 2 directories recursively
syntax- mkdir -p directory name/new directory

 <h2>mv(move) </h2>
to rename file
syntax- mv old_filename new_filename

to move file
syntax- mv filename where to move

can move and rename it 
syntax- mv filename/path(where to move)/rename filename

 <h2>cp(copy)  </h2>
copy file
syntax- cp path

cp directory recursively
syntax- cp -r path 

 <h2>delete </h2>
syntax-rm filename

syntax- rm -r foldername
to wipeout folder
