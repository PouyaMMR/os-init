# **Command Line Options**

Exa’s options are almost, but not quite, entirely unlike `ls`’s.

## **Display options**

- **-1, --oneline**: Display one entry per line

- **-G, --grid**: Display entries as a grid (default)

- **-l, --long**: Display extended details and attributes

- **-R, --recurse**: Recurse into directories

- **-T, --tree**: Recurse into directories as a tree

- **-x, --across**: Sort the grid across, rather than downwards

- **-F, --classify**: Display type indicator by file names

- **--colo[u]r**: When to use terminal colour

- **--colo[u]r-scale**: Highlight levels of file sizes distinctly

- **--icons**: Display icons

- **--no-icons**: Don't display icons (always overrides --icons)

## **Filtering options**

- **-a, --all:** show hidden and 'dot' files

- **-d, --list-dirs:** list directories like regular files

- **-L, --level=(depth):** limit the depth of recursion

- **-r, --reverse:** reverse the sort order

- **-s, --sort=(field):** which field to sort by

- **--group-directories-first:** list directories before other files

- **-D, --only-dirs:** list only directories

- **--git-ignore:** ignore files mentioned in .gitignore

Passing the `--all` option twice also shows the `.` and `..` directories.

## **Long view options**

These options are available when running with `--long` (`-l`):

- **-b, --binary**: list file sizes with binary prefixes

- **-B, --bytes**: list file sizes in bytes, without any prefixes

- **-g, --group**: list each file’s group

- **-h, --header**: add a header row to each column

- **-H, --links**: list each file’s number of hard links

- **-i, --inode**: list each file’s inode number

- **-m, --modified**: use the modified timestamp field

- **-S, --blocks**: list each file’s number of file system blocks

- **-t, --time=(field)**: which timestamp field to use

- **-u, --accessed**: use the accessed timestamp field

- **-U, --created**: use the created timestamp field

- **-@, --extended**: list each file’s extended attributes and sizes

- **--changed**: use the changed timestamp field

- **--git**: list each file’s Git status, if tracked or ignored

- **--time-style**: how to format timestamps

- **--no-permissions**: suppress the permissions field

- **--octal-permissions**: list each file's permission in octal format

- **--no-filesize**: suppress the filesize field

- **--no-user**: suppress the user field

- **--no-time**: suppress the time field

Some of the options above accept parameters: 


- Valid **--color** options are **always**, **automatic**, and **never**.

- Valid sort fields are **accessed**, **changed**, **created**, **extension**, **Extension**, **inode**, **modified**, **name**, **Name**, **size**, **type**, and **none**. Fields starting with a capital letter sort uppercase before lowercase. The modified field has the aliases **date**, **time**, and **newest**, while its reverse has the aliases **age** and **oldest**.

- Valid time fields are **modified**, **changed**, **accessed**, and **created**.

- Valid time styles are **default**, **iso**, **long-iso**, and **full-iso**.