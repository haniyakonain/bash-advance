# bash_advance
shell / cli (command line interface)
shell -> prompt -> instruction to os

ls options(for details, timestamp, etc)

ls -l 
for details
it has permission,number of reference,owner,group owner,size in bytes,last modifies date and timestamp and name of directory
syntax- ls -l fiename

ls -R 
details of sub directory
syntax- ls -R subdirectory name 

ls -t
for timestamp
(can combine commands like ls-lt)
syntax- ls -t fiename

ls -la 
for seeing hidden file name
syntax- ls -la filename

ls -lr fiename
reverse format of what it was modified

ls -s 
for size
syntax- ls -s filename

ls -lR | grep.
recursively grep or give
syntax-ls -lR | grep.filename

ls *.
wildcard
syntax- ls *.filename

ls ..
all folders/files
syntax- ls ..

cat (concatenate)
> is forward operator

cat > 
for adding data
syntax- cat > filename

cat >> 
append data at end of file
syntax- cat >> filename

&&
combine command
syntax- command1 && command2 && command3

mkdir -p 
for creating 2 directories recursively
syntax- mkdir -p directory name/new directory

mv(move)
to rename file
syntax- mv old_filename new_filename

to move file
syntax- mv filename where to move

can move and rename it 
syntax- mv filename/path(where to move)/rename filename

cp(copy) 
copy file
syntax- cp path

cp directory recursively
syntax- cp -r path 

delete
syntax-rm filename

syntax- rm -r foldername
to wipeout folder
