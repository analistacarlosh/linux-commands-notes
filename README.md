# linux-commands-notes
My useful linux commands that some times I need to use.

## Basics commands line on vi bash Linux

- `Ctrl + A: go to the beginning of line`
- `Ctrl + E: go to the end of line`
- `Ctrl + F: move forward one character`
- `Ctrl + B: move backward one character`

## Search some text inside of files

`grep -rnw '/path/to/somewhere/' -e 'pattern'`
- -r or -R is recursive,
- -n is line number, and
- -w stands for match the whole word.
- -l (lower-case L) can be added to just give the file name of matching files.

## Find a directory on SO
`find / -type d -name {directory-name}`

## Check the version of SO
git `
