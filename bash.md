Task 1 
Time taken : 2 hours 
In this task first asked the user what would you like to do by assigning the values 1,2,3,4,5 to addition,subtraction,multipliction,division and average respectively.
using the code 
echo -n "Enter what would you like to do (1: Add, 2: Subtract, 3: Multiply, 4: Divide, 5: Average): read n
Took two values of input: 
using the code 
echo -n "Enter the value of the first number: read x
echo -n "Enter the value of the second number: read y
Then took cases for each value of n 
if ((n==1)); then
a=$(($x + $y))
echo "The sum of two numbers is: $a"
elif ((n==2)); then
b=$(($x$y))
echo "The subtraction of two numbers is: $b"
elif ((n==3)); then
c=$(($x * $y))
echo "The multiplication of two numbers is: $c"
elif ((n==4)); then if ((y != 0)); then
d=$(($x / $y))
echo "The division of two numbers is: $d"
else
echo "Еггог: Division by zero is not allowed."
echo "Еггог: Division by zero is not allowed."
fi
elif ((n==5)); then
avg=$(($x + $y))
avg=$(($avg / 2))
echo "The average of the two numbers is: $avg"
else
echo "Invalid option selected."
fi

Task 2 
Time taken: 1 hour 
Here first read a number.stored rev as 0.
The limit is kept as x is greater than 0.
To reverse the number here we first get the remainder when divided by 10 and store the value in s.The divide the nu,ber by 10 to get the quotient.Afyter reversing if the 
temp number is same as that of the number stored in reverse then the number is a palindrome otherwise it is not a palindrome.

#!/bin/bash
read -p "Enter a numbeг:
temp=$num 
rev=0 num
while [ $num gt 0 ]; do 
s=$((num % 10)) 
num=$((num / 10)) 
rev=$((rev * 10+ s ))
done
if [ $temp -eq $rev ]; 
then echo "The number is a palindrome" else
echo "The number is NOT a palindrome"
fi

Task 3 
Time taken : 2 hours 
The task here was to rotate the letters 
#!/bin/bash
rot13() {
echo "$1" | tr 'A-Za-z' 'N-ZA-Mn-za-m'
}
echo "Welcome to the ROT13 Encoder/Decoder!"
echo "Choose an option:"
echo "1. ROT13 Encode"
echo "2. ROT13 Decode"
read -p "Enter 1 or 2: choice
if [[ "$choice" != "1" && "$choice" != "2" ]]; then echo "Invalid choice. Please enter 1 ог 2."
exit 1
fi
read -p "Enter the text: user_input
if [[ "$choice" == "1"]]; then encoded=$(rot13 "$user_input") echo "Encoded text: $encoded"
else
decoded=$(rot13 "$user_input")
fi

Task 4 : 
Time taken : 30 minutes 
Here the task was to find wether the file persistance exists or no.The code check_file_presence() is used to check wether the file exists.The code { if [ -f "persistence" ] is
used to denote which file we need to find.
#!/bin/bash
check_file_presence() { if [ -f "persistence" ]; then
echo "The file 'persistence' exists."
else
echo "The file 'persistence' does not exist."
fi
{
