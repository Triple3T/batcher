# batcher
Execute single-input program with plural files  
If the program only takes one file at a time and there's too many files to execute with,
this program can be helpful to execute with all target files automatically.

## How to
Compile and drop executable file to target folder.  
Open cmd, and type this command(Windows):
` dir <name>.<extension> /b | <batcher.exe> <executable.exe>`  
- `<name>` is the name of the files. for example: `*`  
- `<extension>` is the extension of the files. for example: `bin`
- `/b` makes `dir` command to print the files' name only.
- `<batcher.exe>` is the executable file from *this repository* that compiled above.
- `<executable.exe>` is the single-input program executable the files that match `<name>.<extension>`.

Example command: `dir *.bin /b | batcher.exe cutter.exe`  
This command executes cutter.exe for all *.bin files in target folder.  
