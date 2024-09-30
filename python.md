Task 1 
Time taken : 30 minutes 
First the palindrome is defined using def is palindrome(s): 
The code first takes  in the string s using x = input("Enter the string: ") then returns the reverse of it by using [::-1] ,the line -1 to reverse the string.
If the x is palindrome it prints String is palindrome otherwise it prints string isnt palindrome.


def is palindrome(s): 
ss.replace(" ", "") 
return s == s[::-1] 
x = input("Enter the string: ")
if is_palindrome(x): 
print("String is a palindrome!")
else: 
print("String isn't a palindrome!")

Task 3
Time taken : 30 minutes 
Here the two string input is taken using.Then each word is sorted and converted to lower case.If the sequence is changed and if both are equal then both are anagram.
The task was easy however I took time in order to find the errors in it.

s1 = str(input ("Enter string 1: ")) 
s2 = str(input ("Enter string 2: "))
s1 = sorted(sl.lower()) 
s2 = sorted(s2.lower())
def isAnagram(): 
if (sl == s2):
return "True"
else:
return "False"
print(isAnagram())

Task 4
Time taken : 30 minutes
The task here is to count the vowel.Here the vowels are defined initially 

def vowel count 
(str): count = 0 
vowel = set("aeiouAEIOU")
for alphabet in str:
if alphabet in vowel: 
count = count + 1
print("No. of vowels:", count) 
str = str(input("Enter the string:")) 
vowel count (str)

Task REQUEST PROTOCOL:
import requests
def check website status (url):
try:
response requests.get(url) if response.status code == 200:
=
print (f" [UP] (url) is up and running.")
else:
print (f"[DOWN] (url) returned status code (response.status_code).")
except requests.exceptions.RequestException as e:
print (f" [ERROR] Could not connect to (url). Error: {e}")
if name == main
website_url = input ("Enter the website URL (including http:// or https://): ") check website status (website url)
