## picoCTF2021
 1. Obedient Cat
 * Just have to download the file and copy the flag.
 2. Netcat
 * First I connected to $ mercury.picoctf.net 43239 using nc command.
 * It gave me an list of numbers which were ASCII values for text.
 * Then I decoded them to obtain the flag.
 3. Static ain't always Noise
 * Download static file and bash script
 * using ./ltdis.sh static , the flag is copied to another file called static.ltdis.strings.txt
 * now cat that file to obtain the flag.
 4. Tab, Tab, Attack
 * Unzip file using unzip function
 * using ls list all folders
 * navigate through them using cd <filename>
 * Find executable file fang-of-haynekhtnamet and use ./ to run it.
 * Flag obtained
 5. Magikarp Ground Mission
 * Connect to server by ssh ctf-player@venus.picoctf.net -p 50713 and 6d448c9c as the password
 * Using ls lists 1of3.flag.txt instructions-to-2of3.txt 
 * With cat 1of3.flag.txt, we get "picoCTF{xxsh_"
 * cat instructions-to-2of3.txt says " Next, go to the root of all things, more succinctly `/`"
 * I typed in cd .. to go back a directory then ls -a and came across 3of3.flag.txt
 * cat 3of3.flag.txt gave "5190b070}"
 * I kept going back (with cd ..) and listing the files and directories (ls -a) until 2of3.flag.txt appeared.
 * cat 2of3.flag.txt gave "0ut_0f_\/\/4t3r_"
 6. Python Wrangling
 * Use python -d flag.txt.en
 * Asks for password and after inputting password flag is obtained.
 7. crackme.py (Reverse Engineering)
 * I opened the file with IDE and went through the code.
 * It said secret of client is bezos_cc_secret = "A:4@r%uL`M-^M0c0AbcM-MFE055a4ce`eN"
 * Next part of the program showed that the text was ROT47 encrypted.
 * I used an online ROT47 decoder on "A:4@r%uL`M-^M0c0AbcM-MFE055a4ce`eN" to obtain the flag.





