# Task 0. Hello World
# echo "Hello, World"
# it will print or display Hello, World

# Task 1. Confused smiley
# echo "\"(Ôo)'"
# it will print or display "(Ôo)'

# Task 2. Let's display a file
# echo "$(cat /etc/passwd)"
# it will print or display the content of the file passwd in /etc directory

# Task 3. What about 2?
# echo "$(cat /etc/passwd /etc/hosts)"
# it will display the content of the 2 files (passwd & hosts) in a different directories at the same time.

# Task 4. Last lines of a file
# echo "$(cat tail -n 10 /etc/passwd)"

# Task 11. Don't just count your directories, make your directories count
# find . -mindepth 1 -type d | wc -l
# find -> finds directories and files on a filesystem
# . -> it start searching from the current directory
# -mindepth 1 -> it finds all directories and subdirectories except the current directory.
#-type d -> it will only find directories and subdirectories (not included files)
# wc -l -> it performs line count on the output of the find.

# Task 12. What's new 
#