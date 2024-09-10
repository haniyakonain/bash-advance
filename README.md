# bash_advance
shell / cli (command line interface)
shell -> prompt -> instruction to os

ls options(for details, timestamp, etc)

ls -l fiename
for details
it has permission,number of reference,owner,group owner,size in bytes,last modifies date and timestamp and name of directory

ls -R subdirectory name 
details of sub directory

ls -t fiename
for timestamp
(can combine commands like ls-lt)

ls -la filename
for seeing hidden file name

ls -lr fiename
reverse format of what it was modified

ls -s fiename
for size

ls -lR | grep.filename
recursively grep or give

ls *.filename
wildcard

ls ..
all folders/files

cat (concatenate)
> is forward operator

cat > filename
for adding data

cat >> filename
append data at end of file

&&
combine command

mkdir -p directory name/new directory
for creating 2 directories recursively

mv(move)
mv old_filename new_filename
to rename file

mv filename where to move
to move file

mv filename/path(where to move)/rename filename
can move and rename it 

cp(copy) 
copy file
cp path

cp directory recursively
cp -r path 

delete
rm filename

rm -r foldername
to wipeout folder
