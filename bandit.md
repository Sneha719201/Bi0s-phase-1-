bandit task 0 - 1
The time taken was 1/2 an hour.I took time to figure out how to write the starting part ssh bandit0bandit.labs.overthewire.org -p 2220 basically the default.
Then I had to understand how to use ls which is list all the files to know in which directory i am in.The next commmand used 
was cat which stood for categorize the directory in order to read the readme file whoich consisted of the password.
bandit task 1 -2 
The time taken for this task was 20 minutes.Next I logged in into task 1 where in  I had to get the password from a - file in the readme directory.- file is something that
cant be read by cat - so i had to use ./- instead to get the password.
bandit task 2 -3 
The time taken for me to solve this task was 10 minutes.The password was saved in file "spaces in this filename" which was not a one word filename so it was not categorisable 
therefore i had to put the filename in double quotation instead to show that is was indeed a single file.
bandit task 3 - 4
The time taken for me to solve the problem was 30 minutes.First i categorized inhere directory,Then i did ls -alps instead of ls to find out the directory inside which inhere/ 
was present.Next I changed the directory to inhere to access the files.There was only one file in ASCII code so i categorized it to get the password.
bandit task 5 - 6
The time taken for me was 30 minutes. I had to find the file with file size 1033c so i used ./size 1033c to figure out the file in the directory then categorizing the file gave 
me the password.
bandit task 6 - 7
Time taken : 30 minutes
This time new command had to be used pwd that is used to display command to show the whole path to the file and then use the file size to identify the file.Next i had to 
categorize the file to access it.
bandit task 7 - 8 
Time taken : 40 minutes 
The function grep had to be used in order to find the password which was next to the word millionth. So the command used was grep 'millionth' data.txt
bandit task 8 - 9 
Time taken: 40 minutes
Here i had to use the man uniq to find out what this function is used for.The code cat data.txt |sort | uniq -u to sort the data in file data.txt and then find out the unique 
part.
bandit task 9 - 10:
Time taken : 50 minutes 
In this task i had to find text with strings and identify the password.The code used here was string data.txt to access the password from the file data.txt.
bandit task 10 - 11:
Time taken : 50 minutes
In this task new command base64 was used as base64 data.txt -d to encode the data in it in binary format and decode it.The password was encrypted in it which i had to access.
bandit task 11 - 12 
Time taken: 30 minutes
This task was a bit difficult for me. The task to rotate the position by 13 positions.Since m is the 13th letter it swaps starts from n-z and next from a - m so the code used 
here was cat data.txt | tr a-zA-Z n-za-mN-ZA-M to rotate position of the letters.
bandit task 12 - 13:
Time taken : 1 hour 
This task was difficult for me had a lot of blockers and lengthy too.Firtsly created a temporary directory using code mktemp -d /tmp/SnehaXXXXXX
Then copied data of file data.txt to the temporary directory.Then changed the directory to the temporary one to work on it.Used the xxd -r ( xxd -r data.txt >) bandit command
to reverse it to binary format.Next moved the data into .gz format.Next used the command gzip to compress the files.Next moved the files to .bz2 format to compress files 
efficiently.I did the same with all the files present to find which was in ASCII text (password)  cat data8.
bandit task 13 - 14 :
Time taken : 1 hour 
The task was getting comparitively difficult as I had to get private ssh key to access next level. Used the commands cat /etc/bandit_pass/bandit14 to pass through the level .
bandit task 14 - 15:
Time taken : 1 hour 
Used code telnet localhost 30000 to connect to the local host.Then used the code nc localhost 30000 in which nc stands for network connection to local host 30000 to access the 
password.













