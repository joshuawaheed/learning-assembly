# Learning Assembly

## Setup the DASM Assembler

*STEP 1*
> Download the DASM Assembler from https://dasm-assembler.github.io/.

*STEP 2*
> Open your terminal and cd to the directory where the DASM Assembler has been downloaded.

*STEP 3*
> Run the following command to unzip the assembler. 
>
> ```
> tar -xzf dasm-2.20.14.1-osx-x64.tar.gz
> ```
>
> Notes:
> - This example is uncompressing the DASM Assembler for the mac operating system.
> - The command might vary for the operating system you are installing the DASM Assembler on.
> - Do an internet search to look for alternative uncompress options if this step does not work.

*STEP 4 (optional)*
> Copy the uncompressed dasm folder to the user local bin folder. This will allow the dasm command to be run from any directory on a mac or linux machine.
>
> ```
> cp dasm /usr/local/bin
> ```
>
> Notes:
> - If you don't do this step, you can run the dasm command from the directory where you have saved it.
> - This might be different in windows.
> - I think for windows, you can:
>   - Move the dasm folder to your preferred location
>   - Make an environment variable point to the preferred location

*STEP 5*
> Compile an assembly file by going to a directory with a file that has the extension .asm by writing the following command in the terminal.
>
> ```
> dasm <filename>.asm -f3 -v0 -o<filename>.bin
> ```
>
> Notes:
> - -f3 is a requirement for the 6502 processor
> - -v0 is setting error messages to zero
> - -o is what we want the file name of the output to be for the binary

## Setup the Stella Emulator

*STEP 1*
> After completing your setup of the DASM Assembler and compiling your code, download the Stella emulator from https://stella-emu.github.io/downloads.html.

*STEP 2*
> Install the emulator.

*STEP 3*
> Run the emulator and then go to the bin file that you created using the DASM Assembler.

*STEP 4*
> Double click on the bin file.

*STEP 5*
> Click on ` on the keyboard to open the debugger.
