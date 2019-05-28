### grep search-phrase filename
returns the lines that contains "search-phrase"

### grep search-phrase filename1 filename2 filename3
search multiple files for the "search-phrase"

### grep search-phrase *.md
wild card search

### grep -r search-phrase foldername/subfoldername
searches recursively, explores all files, sub folders and files within them

### find dirname -name "*.php"
searches all php files in specified directory could give . for current directory

### find dirname -name "*.php" | xargs
xargs takes its input and runs a command on it, by default echo

### find dirname -name "*.php" | xargs grep describe
searches for the word describe in the find result files

### grep -r --include="*.php" "search-text " foldername
same result as above using grep

### git grep search-text
finds the search text only in repository files, ignore .gitignore

### grep -n search-text *.php
tells the line number along with the found text

### grep -A 2 search-text *.php
gets separated blocks along with 2 lines of context along with the result

### grep --color "h." readme.md
searches for h (any single character and it can be anything)

### grep --color "\.com" readme.md
escape . special meaning

### grep --color "(.*)" readme.md
anything between (any text)

### grep --color -E ".com" readme.md
you do not need to escape anything in regex



