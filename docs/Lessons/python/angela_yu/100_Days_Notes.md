# 100 Days of Python

### Udemy Angela Yu

## Day 3

### RANDOM 

``` python
import random
random_integer = random.randint (1, 10)
```




41, LISTS 
 create a module called my-module.py 
pi = 3,14. 
in main, py 
import my-module 
print (my-module, pi) 
random_float = random, random () # 0 To 1 
Not including I 
to get a float between 0 and 5 just multiply *5. 
Use a seed 
toget better random numbers. Seed needs to be something random itself. 
list_var = ["item\" "item 2", "item 3"] lists have an order-number is first 
Ø 
name_of_list [index] To Refer to items in list negative indexes = -1 last item in list, -2 next to tong list-var, append("item4") => appends to end of list." , extend (another list) Zadds list to end of list 
43 INDER ERRORS 
48 FOR LOOPS 
100 DAYS of PYTHON P.4. 
TRYING TO ACCESS ITEM Larger 
than length 
of list, ofF BY ONE ERRORS FORGETTING index starts at zero. 
nested lists 
list 3 = [list1, list 2] 
print (list 3) 
[[ 1, 2, 3, 4], [5, 6, 7, 8]] print (list 3 [0,3]) = 4 
for x in list: 
1,3 
778 
INDEX 
print x 

# PRINTS CONTENTS OF LIST (NOT THE 51 range range generates numbers to loop through 
for number in sange (1, 10): #doesn't include 10 so prints 1 to 9 range (6) Oto 6 -zero assumed. range (1, 10, 3): steps by 3 so 1, 4, 7 random, choice (list) graps a random item 
from the list. 
list, append (I) - appends item to list 
random, shuffle (st) shuffles a last 
57 FUNCTIONS LOTS OF BUILT IN FUNCTIONS; eg, int(), ten () 
def our function (parameters): #define function. 
Indented code block 
59 INDENTAT Our-function # To execute function 59-INDEN- spaces or tabs both work, but not together 
STYLE GUIDE SAYS 4 spaces for indent. 
TATION 
most editors can sub spaces when press tab, 
6. While loops 
100 DAYS OF PYTHON P.5 
number hurdles 26 
while true-condition: while number hurdles >0: 
repeat 
Until 
false 
jump () number_hurdles -=1 
78. FUNCTIONS put variable inside parens in det stmt. 
WITH INPUTS 
then include a value when you call the function 
paramete is what's defined in the function 
def my_func (parameter) 
argument is what you call the function with 
my-func (argument) 
80. POSITION multiple parameters Just seperate with US Keyword 
commas - up to now these are positional arguments. 
Keyword arguments 
def 
my-func (name, location): 
my_func (name = "John", location = math, ceil will round a number up. gallons = math, ceil (area (cover) 
"Texas") 
list. index (list_item) returns index of 1st match 
index = alphabet, index ("c") => index = 2 
89. DICTIONARY KEY: VALUE PAIRS. 
Dete DIVE Programming - dictionary = {"bug": "Det_OF_BUG", 
"Runction": "Def_of_ function" } formatted usually as 
name_of_dict = { 
3 
KEY: VALUE, 
in list 
KEY: value, #(YES a comma after last valve) 
100 days of code 
7 cont To access: 
P.6 
Print (programming - dictionary ["Bug"]) 
To add new entry to dictionary 
programming dictionary ["Loop"] = "def of loop Create empty dictionary 
empty_dict = { } Wipe existing dictionary 
programming- dictionary = {} 
Edit item in dictionary 
" 
programming - dictionary ["Bug"] = "new definition Loop through dictionary 
for thing in dictionary: 
print (thing) = only prints Keys 
So can do 
91 nest 
{ 
LISTS & 
Dictionaries 
る 
Key 
for thing in dictionary: 
print (Key) 
# print key 
print (dictionary [key]) # print valde, 
Key: [list] 
Key: Edict} 
travel-log = { 
пи 
il 
France": [ "Paris", "Lille", "Dijon"] 
"Germany": ["Berlin", "Hamburg", "Stuttgart"] 
100 days of Python p.7 
Il cont Fiested dictionary = { 
97 FUNCTIONS 
3 
"France": { "cities-visited": ["Paris", "Lille", 
"total_visits": 123, 
"Dijon 
"Germany": { "cities-visited": [ "Berlin", "Hamburg", 
"Stuttgart], "total-visits": 73, 
she then changed to a 
list containing dictionaries, just replace outer 2 curly braces with [] 
with outputs Using return Keyword to return 
output from the function output = my-function () 
98 MULTIPLE 
RETURN 
VALUES 
def format-name (f_name, 1-name) # function title built in to python. 
f_name = fname.title() 
1_name = 1_name, title ( 
return f-name + " " + _nante 
ப 
print (format-name ("+Erry", "dU+Chεr")) 
could return an f string 
return "f"&f-name} { 1-name}" 
ANY code after return doesn't execute Can have multiple returns in if stmts. 
пор 
И 
100. 
100 days Python P. 8. 
if x: 
else 
return x 
return Y 
Can have empty return - why? 
DOCSTRINGS Way to create documentation 
DAY 12 
14 GLOBAL 
LOCAL 
must be first line in a function & contained 
3 double quotes, Can be multiple lines. take 1st & last name and format as title 
in 
ALLON 
local 
0170/1 
set Variables a inside function are to that function To make a variable "global" declare it outside 
all functions -applies to nested functions too - 
anything you give a name to 
To modify a global variable inside a function 
have to use stmt global var_name 
Bad form to name variables inside function same 
as another vas outside the function. Using global stat in a function is discouraged. 
Don't modify global 
you can read the 
read the global var, modify it and return it, 
117. GLOBAL Naming convention for constants is all UPPER CASE 
Constants 
100 DAYS Python P. 9 
Dory 12 con't. number guessing game 
DAY 13 
easy 10 tries, hard 5, number between 1, 100, 
Text to ascil generator-online 
DEBUGGING 
-DESCRIBE THE PROBLEM MAKE SENSE OF WHAT'S 
GOING ON 
- REPRODUCE THE BUG = when bug is intermittent 
-PLAY COMPUTER 
-FIX ERRORS THE EDITOR SHOWS 
~print is your friend-print variables to check them -DEBUGGERS- can set breakpoints -pythontutor.com 
Visualize setting. 
-run program as you're developing it, -when all else fails stack overflow, after 
first searching stack overflow, 
DAY 14. HIGHER-LOWER Game 
higher-lower-final appbrewery, replirun. -Breakdown into smaller pieces. 
-make to do list of what needs to be done - put those comments todos into comments -write code 
Starter code 3 files, main (empty) art (logo & 
vs), game-data (list of dictionary entries), Keys: name, follower count, description, country 
DAY IS 100 DAYS Python P.10 
WAY 15 install python & set 
JULY 14 on UBUNTU 21.04 
DAY 16 
up 
local development environment 
UBUMATE FROM JETBRAIN'S 
Pycharm IDE. I installed on ARCH from repo 
FEATURES - Spell check for english - underlines with squiggle -hover & get suggestions -More space to develop - you can have tabs 
& right click on tab & can window 2 screens -Built in linter-clean up code -style guide Squiggles again & hover to see why 
- 
SPLIT 
-Show history - can see edits made (12 hrs ?) 
LINKS TOO 
- Structure pane-shows functions & variables Foo -refactor rename - able to change variable 
or function name everywhere it's used 
-todo tracking -tab at bottom 
# TODO: 1. Print report 
-alt shift - select multiple lines for multi line 
cursors 
object Oriented programming. 
Split larger task into smaller pieces. pieces can be worked on at separate times or 
by separate teams 
attributes-describe obect -usually variable methods - things object condo - functions both attached to aspecific object. 
class is overall decription 
- 
object generated from class can be multiple 
objects per class 
Jity 16 
cont 
100 Days Python Pill class-blueprint 
- 
object - created from blueprint car 1 = Car Blueprint () 
in Python 
under 
scores 
classes name each word capitalized no cart is object Car Blueprint () is class there is a Turtle class inside the turtle module 
import turtle 
Using external 
object 
timmy 
OR 
= 
turtle. Turtle () #new object timmy 
from turtle import Turtle, Screen timmy = Turtle() 
another object turtle 
Class my_screen = Screen () # screen is where draws 
ttribute: print(my-screen, cand height) #Canvas height attr 
methods 
my_screen, exit on click () #method 
- 
program runs until we click on screen timmy, shape ("turtle") change shape of timmy obj. 
Python Package Index pypi.org 
to install under Pycharm -go to settings, 
click on project, then project interpreter + button bottom left, search for package, select it & click install. 
WAY 17 
100 Days of Python. 
P12 
Create your own custom classes 
class Car: #where car is name of class 
-pascal case all words start w/ upper case my_buick = Car() # create an object 
can use pass Keyword to skip function or class 
Creating class attributes -variable attached to 
an object. 
class User: 
Pass 
User_1 = User() 
user_1; username = "Angela" # creates attribute usernam #would have to do this for every user-error 
prone easy to mispell a name, etc. 
Constructor - initialize (construct) the object class Car: 
def __init__(self, seats) : nome- 
# initialize attributes -don'tclude self self, seats = seats 
class User: 
special function 
in Ball creating object 
new 
def __init__(self): called every time object 
When you're creating a new obect 
you 
must 
provide the parameters defined in __init__ 
100 days of python 8,13 
DAY 17. Can have default values that don't have an 
associated parameter 
cont 
class User: 
def __init__(self, user-id, username): 
self.id = user-id 
self, user name = username 
self, followers = 0 
user_ = User ("001" "angela") user_2 = User ("002", "jack") 
Create methods 
class Car: 
def enter race-mode 
self, seats = 2 
=2 
my-car, enter-race- mode 
back to user 
def follow (self, user): 
user, followers +=1 
+ 
self. following → = | 
user-1. follow (user_2) 
(self); 
# 
○井 
#self required. 
open trivia database was ap; to generate 
questions - json format 
correct 
use question & question_answer 
Del 18 
100 Days of Python P.14 Turtle module 
HARO from turtle import Turtle, Screen timmy_the_turtle Screen ( 
screen = 
= Turtle () 
screen, exiton click () ← needs to be at bottom 
turtle docs on python, ond 
timmy-the-turtle shape ("turtle") 
-lots of other shapes in docs, 
google does 
a better job of searching stack ovest hour than the stack overflow built in search 
timmy_the_turtle ("red") 
-use TK color strings or #hex or 
forward, backward, right (angle), left (angle) 
importing modules 
import turtle 
tim = 
turtle. Turtle() 
from turtle import Turtle 
tim = Turtle () 
# most obwous where stoff comes from 
from turtle import * # hard to see where stuff 
tim = Turtle () 
comes from, Not good code 
100 days of Python 1.15 
DAY 18 cont Aliasing modules 
DAY 19 
import turtle as + 
tim 
= +. Turtle () 
Some modules have to be installed they don't 
come packaged with python 
pypi.org 
in Pycharm hover & gives prompt to install heroes 
tuple - like list but (instead of [] -immutable pencolor for turtle rgb tuple 
colorgram - extracts colors from images colorgram, extract (image, number_of_colors, 
Turtle Event Listeners 
in Turtle docs - Under Screen Events 
listen method - starts listening screen, listen () 
screen, onkey (move forwards (key = "space", 
fun = move forward) # no parameter/parens. def move-forwards (): 
tim, forward (10) 
screen. exiton click () 
any 19 
cont 
100 Days of Python. note you're passing 
as a parameter 
P. 16 
a function to a 
function 
A function that can work with other functions 
is called a higher order function, 
think of simple calculator 
def add (nl,n2): 
def Subtract (nl, na): 
det multiply (nl,n2): def divide (nl,n2): 
def calculator (nl, n 2, func): return func (n),n2) 
she recommends using n't create yourself, 
Keyword arguments for 
+ 
methods you 
didn't 
especially when the order really has no meaning, 
Can create many objects from one class 
called separate instances of the class 
screen. setup (500, 400) 
八 
八 
(width=500, height = 400) # recommended 
text input - popup to enter text--return text 
turtle goto (x = ~250, x = -100) 
yaxis center ó 
↑ positive, & negative. so 200 to -200 in our setup above xaxis center o→ positive < negative go to - don't use very edges of screen. 
Je, 19 
cont 
100 days of Python P.17 
But easier 
tim = Turtle Ishape = "turt le") 
100 DAYS PYTHON DAY 27 TKINTER 
247 Create Windows & Labels 
import +kinter 
window = +Kinter, TK() #First Window, mainloop() 
Title 
# Last-event loop 
window, title("My first GUI Program") 
Minimum Size 
window, minsize (width = 500, height=300) Label-first create the label- then how to display it 
my-label = + Kinter. Label (text="Label"") my- label. pack() 
Label Font -add to label definition 
font=("Arial", 24, "bold") 
Pack method 
my-label, pack (side = "left") 
-also bottom, right, top

#python
#angelayu
#udemy

#tagcheck
#tagcheck
#tagcheck
#tagcheck
