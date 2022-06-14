#crab

crab is a low level programming language.

a main .crab file will call on .crabscript files in the sequence they are called.

the start of a script file would be written as:

script script_name <Args[] {--arg1 : arg arg1 : }, crun[] {run_command}, cend[] {end_command} > {

then you have have an initiate file by writing:

ini[ svar[var varname : value], cdata[customdataholdname = datastorageformat], access [ sys.display[] ] ]

access would give the program access to certain hardware.

then main would be written as:

script_name.main(Args[], crun[], cend[], svar[], cdata[], access[], em[script_name.error]) {

you also need an error manager, this would be written as:

script_name.error(Args[], crun[], cend[], svar[], cdata[], access[], main[script_name.main]) {

then, you need an onquit manager, written as:

script_name.onquit(Args[], crun[], cend[], svar[], cdata[], access[]) {

then in the main file, you would start it as:

Crab Main{

then you would list the script names after run:

run script_name

scripts can also be run from the console using the run command.

scripts can run other commands using 

crab.scripts.run(script_name)
