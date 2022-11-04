# Javascript-Topics
I have written notes for javascript concept by thapa technical javascript


Challenge 1:Rules in naming variables
state whether these naming practices are valid or not
var _myName="vinod"
var _1my__Name="abcd"
var 1myName="thapa";
var $myName="thapa technical"


var _myName="vinod"
console.log(_myName);
var _1my__Name="abcd"
console.log(_1my__Name);
var 1myName="thapa";
console.log(1myName,"not valid");
var $myName="thapa technical"
console.log(1myName);

Challenge 2:Output of following

10 + "20"=1020
9-"5"=4
"java"+"script"=javascript
""+""=space itself
""+0=0
"vinod"-"thapa"=NaN
true+true=2
true+false=1
false+true=1
false-true=-1


interview question:

->what is the difference between null and undefined

undefined is a type of instance in javascript
null is an object
where null can be assigned to a variable
but when a variable is assigned nothing it is undefined.

->what is NaN?
not a number is a property of a global object which states when the output of some function or calculation 
is not a legal number.It is global object property which is same as number.It is a variable in global scope.
Even it is used for validation in forms.


Challenge 3:NaN practice

 NaN===NaN(false)(NaN is not a datatype to compare,it is a property)

 Number.NaN===NaN(false i.e, again NaN===NaN)


 Number.isNaN(NaN)(true)


expressions and operator
  
terms:operand and operator

...>assignment operators(=)
 isNaN(NaN)(true)

 isNaN(Number.NaN)(true)
...>arithmetic operators(+,-,/,*,%,++x,x++,--x,x--,**(exponentiation operator))
...>comparison operators(>,<,>=,<=,==,===,!=)
...>logical operators(&&,||,!,!!) 
...>string operators(+ ->concatenation operator)
...>conditional operator(ternary operator)

challenge 4:

->what will be the output of 3**3(power of symbol i.e.., exponent three cube)127

->what will be the the output when we add a number and a string 3+"22"=322 NaN finally

->write a program to swap two numbers

   let a = 5, b = 10, c;
   c = a; //c=5
   a = b; //a=10
   b = c; //b=5
 
   console.log('a', +a);

   console.log('b', +b);

   console.log('c', +c);

-> write a program to swap two numbers without using third variable

a=a+b; //(a=5+10=15)
b=a-b; //(b=15-10=5)
a=a-b;//(a=15-5=10)

console.log("a",+a);
console.log("b",+b);

->Interview question

-->Difference between == and ===?

   The difference between == and === is that: == converts the variable values to the same type before performing comparison. This is called type coercion. === does not do any type conversion (coercion)
   and returns true only if both values and types are identical for the two variables being compared.

   example:a=5 b="5"

   a==b true
   a===b false



control statements and loops

if ... else


if(condition)

{do this}

else

{do this}

challenge 5:

write a program that works out whether the given year is a leap year or not?

let year;

function leapYear(year){
  if(((year%4 )==0 )&&( year%100!=0 && year%400!=0)){
    console.log(year+" "+"is a leap year")
  }else{
    console.log(year+" "+"is not  a leap year")
  }
}

leapYear(2014);

what is truthy and falsy values in javascript?

if(score=0){
console.log("Yay, we won the game")
}
else
{
console.log("OMG ,we lost the game")

}
}

ans: we have total 5 falsy values in js 
those are(0,"",undefined,null,NaN,false**is anyway false)
except these if you write anything in if condition it will be true.


what is ternary operator?

it can also be called as conditional operator which takes three operands 

e.g: var age=17;((age>=18)? "you can vote": "you cannot vote");


SWITCH STATEMENT:


example:find area of given shape using switch statement

let area,PI=3.142,l,b,r;
function findArea(area,l,b,r){

  switch(area){
    case 'circle':
      console.log("the area of circle is :"+ PI*r*2);
      break;
      case 'rectangle':
        console.log("the area of rectangle is :"+ l*b);
       break;
        case 'triangle':
          console.log("the area of triangle is :"+ l*b/2);
        break;
          default :
          console.log("please enter valid data");
  }
}

findArea("rectangle",5,4,4)



While loop statement:

the while statement creates a loop that executes a specified statement as long as the given condition is true


var num=20;
while(num<=10){
  console.log(num);
  num++;
}


do while loop statement

this first executes the program and then checks the condition


var num=20;
do{
console.log(num);
num++;
}while(num<=10)


For loop statement:


for(var num=0;num<10;num++){
console.log(num);
}

Challenge 6:for loop practice

-> Write a javascript program to print table for given number using for loop?

   var number, result;
   function mulTable(number) {
  for (var i = 1; i <= 10; i++) {
    result = number * i;
    console.log(number + '*' + i + '=' + result);
  }
}

mulTable(8);

functions in javascript:

a js function is ablock of code designed to perform a particular task

=>function definition:

before we use function we need to define it

function definition is also called as function declaration, function statement

function definition consists of following:

1.Name of the function
2.A list of parameters enclosed in parenthesis seperated by commas
3.block of code enclosed in curly brackets

=>Calling functions

Defining a function does not execute it we have to call it or invoke it.


challenge 7:

->What is the difference between function parameters and function arguments?


 function's parameters are the names listed in the function definition
 function 's arguments are the real values passed to the function when it is called.

Why functions?

you can reuse the code .It eliminates the writing of code again and again.

A group of reusable code that can be called anywhere in the program.

=>function expressions :It means create a function and put it into the variable

function sum(a,b){

var total=a+b;
console.log(total);
}

var myTotal=sum(a,b);

=>return Keyword:

when javascript reaches return keyword it stops executing and 
functions often compute a return value.
the return value is returned back to the caller.

function sum(a,b){

return total=a+b;

}

var myTotal=sum(5,9);
console.log(funExp);

=>Anonymus functions:

functions without name

e.g:

It can be same written as function expression but without a name


var myTotal=function(a,b){

return total=a+b;

}
console.log("the sum of two numbers is"+funExp);

========================================================ECMA SCRIPT 6===================================

*****History :

1996:javascript was created

1997:javascript was submitted ECMA international for standardisation ,
     which resulted in ECMAScript

----There are so many updates in javascript since it was handed over to ECMA international but -------
 

2015:It was decided for annual release updates. so ES6 was this much famous and familiar to everyone.


*****Timeline:

2015:ECMAScript 2015 ES6 or ECMAScript 6

2016:ECMAScript 2016 ES7 or ECMAScript 7

2017:ECMAScript 2017 ES8 or ECMAScript 8

2018:ECMAScript 2018 ES9 or ECMAScript 9

2019:ECMAScript 2019 ES10 or ECMAScript 10

2020:ECMAScript 2020 ES11 or ECMAScript 11


*****Services

LET and CONST

TEMPLATE STRINGS

DESTRUCTURING

OBJECT PROPERTIES

DEFAULT ARGUMENTS

ARROW FUNCTION

REST OPERATORS

SPREAD OPERATORS


//***********************************************************************************************

// NOW ITS TIME FOR MODERN JAVASCRIPT

//FEATURES OF ES6


1.let                                const                               var 
                                                 
        
block scope                     block scope                                  function scope
  
can be reassigned               cannot be reassigned                    can be reassigned

mutable                         immutable                                mutable


2.template literals

numTable(8);
function numTable(number) {
  for (let i = 1; i <= 10; i++) {
    let result = number * i;
    console.log(`${number} * ${i}=${result}`);
  }
}

3.Default parameters

4.fat arrow function

const numTable1=(number)=>{
  for (let i = 1; i <= 10; i++) {
    let result = number * i;
    console.log(`${number} * ${i}=${result}`);
  }
}
numTable1(8);

Difference between fat arrow and normal function

                  arrow func                                                normal func
 

syntax: let add =(x,y)=> x+y;                         function add(x,y){return x+y;}

        let add= x=>x*x


arguments binding is different in both

use of this keyword is different in both

new keyword can be used in normal function but not in arrow function


no duplicate parameters in arrow function 



=>Arrays in javascript

when we use var we can store only value if we want to store multiple values in one variable 
then we will use array.
In js we have array class,arrays are prototype of this class.

var friend="maithili"
var friend1="radhi"
var friend2="moksha"

where as in array

var friends=['maithili','radhi','moksha']
INDEX              0        1        2
3 elements starting from indexing from 0;


//WE USE FOR LOOP TO NAVIGATE AN ARRAY

for(var i=0;i<friends.length;i++){
console.log(friends[i]);

}

//After ES6 we have for in and for of loops


for(let elements in friends){
console.log(elements);
}
output :
0
1
2


for(let elements of friends){
console.log(elements);
}
output :
maithili
radhi
moksha

array.prototype.forEach()
call a function for each element in the array.

friends.forEach(function(element,index,array){
console.log(element+"index:"+index+""+array);
})

output:
maithili index:0  maithili, radhi ,moksha
radhi  index:1    maithili, radhi ,moksha
moksha  index:2   maithili, radhi ,moksha


}

//arrays:searching and filter

=>array.prototype.indexOf() is used to search any element in an array.


var friends=['maithili','radhi','moksha']

console.log(indexOf("maithili"))
output:0

var fM=['maithili','radhi','moksha','radhi`swife',];
console.log(fM.indexOf('radhi',2));

output:-1(none is present)

var fM=['maithili','radhi','moksha','radhi`swife',];
console.log(fM.lastIndexOf('radhi',2));

output:2(none is present)

both indexOf() and lastIndexof() gives the index of element but indexOf()is forward search 
and the second one is backward search.


=>arrays:Includes

-->array.prototype.includes()

determines if an element is included in the array or not 
returns true or false as an output.
includes method is case sensitive too.
it doesnot do backward search like lastIndexOf()
method
e.g:var fM=['maithili','radhi','moksha','radhi`swife',];
    console.log(fM.includes('radhi'));

output:true


=>arrays:find()

Array.prototype.find();
returns the found element in the array if some satisfies the testing function if not undefined.
only problem is it returns only one element.

eg:prices=[100,200,300,400,500,600]

prices<400

console.log(prices.find((currentVal)=>currentVal<400));

output:100

=>arrays.findIndex()

returns the found index in the array if there satisfying the condition or -1 if not found.

console.log(prices.findIndex((currentVal)=>currentVal<400));

output:0


=>arrays:filter()

array.prototype.filter()

returns new array containing all the elements of calling array for 
which the provided filtering function returns true.

const prices=[100,200,300,400,500,600];

const newPrice=prices.filter((element,index)=>{return element<400});
console.log(newPrice);

output:[100,200,300]

if no element is present it returns a new empty array


=>arrays:sort()

returns the sorted array.the default sort order is ascending,built

built upon converting elements into strings

then comparing their sequences of UTF-16 code units values.

const months=['March','Jan','Feb','Dec','Nov'];

console.log(months.sort());

output:["Dec", "Feb", "Jan", "March", …]
0: "Dec"
1: "Feb"
2: "Jan"
3: "March"
4: "Nov"

const array=[1,40,10000,3,21];
console.log(array.sort());

[1, 10000, 21, 3, …]
0: 1
1: 10000
2: 21
3: 3
4: 40

if u see 21 is smaller than 3 because of 2 and 3 digits comparison in the one's place.
sort method produces incorrect resullt when sorting numbers 


=>array crud operation


=>array.prototype.push();->adds one or more elements at the end of the array and returns the new
 length of the  array

e.g:const animals=['pigs','cows'];
const count=animals.push('chicken','cats','dogs');
console.log(animals);
console.log(count);//push method returns new length of aarray

=>array.prototype.unshift();

adds one or more elements at the begining of the array and returns the new
 length of the  array
 
e.g: const animals=['pigs','cows'];
const count=animals.unshift('chicken','cats','dogs');
console.log(animals);

=>array.prototype.pop();

removes elements from the end of the array and returns that element.this method c hanges the length of the array.

const animals=['pigs','cows','chicken','cats','dogs'];
const count=animals.pop();
console.log(animals);

=>array.prototype.shift();

removes elements from the begining of the array and returns that element.this method changes the length of the array.

const animals=['pigs','cows','chicken','cats','dogs'];
const count=animals.shift();
console.log(animals);


=>array.prototype.splice();

add or removes elements from the array 

Challenge 10: splice method practice

const m=['jan','feb','march'];

1.add dec at the end of the array

sol:const m=['jan','feb','march'];

const insert=m.splice(m.length,0,'dec');

console.log(m);

2.what is the return value of splice method?

sol:returns the deleted elements in an array

3.Update march to 'March'?

sol:const indexOfMarch=m.indexOf('march')

const update=m.splice(indexOfMarch,1,'March')

console.log(m);

4.delete feb from the above array?

sol:const indexOfFeb=m.indexOf('feb')


const delete1=m.splice(indexOfFeb,1)

console.log(m);

now it returns the deleted feb.


note: if we want to delete the total elements after some particular element then do the following.

const indexOfFeb=m.indexOf('feb')


const delete1=m.splice(indexOfFeb,Infinity)

console.log(m);


INTERVIEW QUESTION:
//what is the solution to make this below condition true?

console.log(a == 1 && a == 2 && a == 3);

const a = { num: 1 };

a.valueOf = function () {
  return this.num++;
};



==============================MAP REDUCE ===================================


array.prototype.map()

let newArray=arr.map(callback(currentValue[,index[,array]]){
//return element for newArray,after executing something
}[,thisArg]);

returns a new array containing the results of calling a 
function on every element in this array.

const array1 =[1,4,9,16,25];


e.g:num>9

let newArray=array1.map((curelem,index,arr)=>{return curelem >9})

console.log(array1);
console.log(newArr);

//how map works and is different from forEach.

let newArr1=array1.map((currentVal,index,array)=>{
  return `Index Of =${index} current value is =${currentVal},of the array:${array}`
})

console.log(newArr1);

output:

[
"Index Of =0 current value is =1,of the array:1,4,9,16,25",
"Index Of =1 current value is =4,of the array:1,4,9,16,25", 
"Index Of =2 current value is =9,of the array:1,4,9,16,25",
"Index Of =3 current value is =16,of the array:1,4,9,16,25", 
…]
0: "Index Of =0 current value is =1,of the array:1,4,9,16,25"
1: "Index Of =1 current value is =4,of the array:1,4,9,16,25"
2: "Index Of =2 current value is =9,of the array:1,4,9,16,25"
3: "Index Of =3 current value is =16,of the array:1,4,9,16,25"
4: "Index Of =4 current value is =25,of the array:1,4,9,16,25"

It is traversing on each and every element by pointing to current element.
by giving a new array and not mutating the original array.

both map and foreach do the same thing but the returned value is different.

another difference between map and forEach is that 
map array method is chainable that means you can attach reduce(),sort(),filter()and so on after performing a map() method on array. 


this is what forEach cannot do  and returns an undefined.



Challenge 9:

1.find the square root of each element in an array?

let array=[25,36,49,64,81]


let newArray=array.map((currentVal)=>
  Math.sqrt(currentVal)
)

output:[5, 6, 7, 8, …]
0: 5
1: 6
2: 7
3: 8
4: 9

2.Multiply each element by 2 and return only those elements which are greater than 10?

let arr=[2,3,4,5,6,8]


let newArr=arr.map((curr,index)=>{
     
    return curr*2
}).filter((curr)=>{
return curr>10
})

console.log(newArr);


Reduce method:

//flatten an array means to convert the 3d or 2d array into a single dimensional array.

the reduce() method executes a reducer function (that you provide) on each element of the array resulting in single output value.

the reducer function takes four arguments:

//previous value,current value,current index,source array

let arr=[6,4,2];

let reducedArr=arr.reduce((previousValue,currentValue,currentIndex,array)=>{
  return previousValue+=currentValue;
})

console.log(reducedArr);

challenge 10:

how to flatten a 2d or 3d array into single dimensional array?

let arr=[

  ['one','two'],
  ['three','four'],
  ['five','six'],
  ['seven ','eight','nine'],


]
console.log(arr);
let newArr=arr.reduce((prevValue,currValue)=>{
  return prevValue.concat(currValue)
})

console.log(newArr);

output:
[Array[2], Array[2], Array[2], Array[2]]
0: Array[2]
 0: "one"
 1: "two"
1: Array[2]
 0: "three"
 1: "four"
2: Array[2]
 0: "five"
 1: "six"
3: Array[3]
 0: "seven "
 1: "eight"
 2:"nine"




["one", "two", "three", "four", …]
0: "one"
1: "two"
2: "three"
3: "four"
4: "five"
5: "six"
6: "seven "
7: "eight"
8:"nine"

2d array converted two a 1 d array
for e.g if its a 3d array it will be flattened then to 1d array
----------------------------------------------------------------------------------
==================================STRINGS========================================

a js string is zero or more characters written inside quotes.

javascript strings are used for storing and manipulating text.

you can use single quotes or double quotes.

strings can be treated as primitives,from string literals or as objects,using the String() constructor.

e.g:let myName="maithili angajala";
    let myChannelName='myra vlogs'
    //let ytname=new String("myra vlogs by maithili");
    
    console.log(myName);
    console.log((ytname))

 
//How to find the length of the string?
String.prototype.length
reflects the length of the string.

let myName="myra vlogs"

console.log(myName.length);


=> Escape character:
 if you want to highlight some string or word in a sentence while assigning to a variable we have to use alternative quotes or backslash.
 
 
 e.g://let anySentence ="this is a "word""; // wrong this way causes error

///*** sol to this is 

//let anySentence ="this is a \"word\"";     // this 

let anySentence ="this is a 'word'";         //or this



=>finding a string in a string

two methods:indexOf(),lastIndexOf()

e.g:

let anySentence ="this is a 'word'";         

console.log(anySentence.indexOf("this",4))

output :-1//checks from index position 4 forward search


console.log(anySentence.lastIndexOf("is",0))

output:-1//checks from index position 0 backward search 

indexOf(searchString: string, position?: number): number
The index at which to begin searching the String object. If omitted, search starts at the beginning of the string.

Returns the position of the first occurrence of a substring.


lastIndexOf(searchString: string, position?: number): number
The index at which to begin searching. If omitted, the search begins at the end of the string.


Returns the last occurrence of a substring in the string.




=>searching a string in a string

search()

search(searcher: { [Symbol.search](string: string): number; }): number
Finds the first substring match in a regular expression search.

let anySentence ="this is a 'word'";        

console.log(anySentence.search( "this"))

output:0

//search method cannot take a second start position argument.

console.log(anySentence.search( "this",4))

output:0 //still the output is 0 no change 

//search method searches for a specific string and returns the matching index for that.

console.log(anySentence.search( "This"))

output:-1


=>extracting string parts

there are 3 methods for extracting parts of a string


slice(start,end)
substring(start,end)
substr(start,length)

slice:

slice(start?: number, end?: number): string
The index to the end of the specified portion of stringObj. The substring includes the characters up to, but not including, the character indicated by end. If this value is not specified, the substring continues to the end of stringObj.

note:original array will not be changed

Returns a section of a string.

e.g:let anySentence ="this is a 'word'";         

console.log(anySentence.slice( 0))

output: this is a 'word'

console.log(anySentence.slice( 0,6))

this i

console.log(anySentence.slice( 0,-2))

this is a 'wor //if -2 is given as end it removes last two letters and returns till the end

..>>challenge 11:Display only 280 characters of a string lke the one used in twitter?

let myActualTweet=mytweet.slice(0,280)//0 to 279 =280

console.log(myActualTweet);

console.log(myActualTweet.length)

substring:

substring(start: number, end?: number): string
Zero-based index number indicating the end of the substring. The substring includes the characters up to, but not including, the character indicated by end. If end is omitted, the characters from start through the end of the original string are returned.


Returns the substring at the specified location within a String object.

note:similar to slice but difference is that its output is different when we give 
negative indexes

e.g:let anySentence ="this is a 'word'";         

console.log(anySentence.substring(3))

output:s is a 'word'


let anySentence ="this is a 'word'";         

console.log(anySentence.substring(7,-2))

output:this is   //it returns the letters from 0th position to the start of the index

substr:

substr(from: number, length?: number): string
The number of characters to include in the returned substring.

Gets a substring beginning at the specified location and having the 
specified length.

note:it doesn't accept negative indexes in the length part it means no output is shown.

e.g:let anySentence ="this is a 'word'";       

console.log(anySentence.substr(3,9))

output:s is a 'w

e.g:let anySentence ="this is a 'word'";         

console.log(anySentence.substr(7,-2))

output: //nothing

so its main use is if we want to extract the last parts or from
backward of the string we can easily do it with substr

e.g:let anySentence ="this is a 'word'";         

console.log(anySentence.substr(-6))

output:'word'



=>Replacing string content

string.prototype.replace(searchFor,replaceWith)

the replace() method replaces the specified value with another
value in a string

let Content="I am maithili angajala and maithili kammila also"

let replaceContent=Content.replace('maithili','Maithili');

console.log(replaceContent);

output:I am Maithili angajala and maithili kammila also

points to remember:

1.replace method doesnt change the string it just replaces the word and returns a new string
2.It changes fisrt found word.

3.By default replace method is case sensitive. //writing MAITHILI (with upper case will not work)



=>Extracting string characters

there are 3 methods:

charAt(position)
charCodeAt(position)
Property access [ ]



charAt() method:

returns the character at specified index position.

let str="HELLO WORLD"
console.log(str.charAt(0))
output:H

charCodeAt() method:

returns the unicode of the character at a specified index in a string 

the method returns UTF-16 code (an int b/w 0 to 65535)

the unicode is a unique number forevery character no matter the platform app or language UTF-8 is a popular unicode encode which has 88-bit code units.


let str="HELLO WORLD"
console.log(str.charCodeAt(0))
output:72

Challenge:12

//return the unicode of the last character in a string

let str="Hello world"

let str="hello world"
let len=str.length-1;
console.log(len)
console.log(str.charCodeAt(len));

output:100


//property access:

ECMA Script 5 (2009) allows property access [] on strings

let str="hello"
console.log(str[0]);
output:h

//other useful methods:

toUpperCase();
toLowerCase();
concat();->joins two or more strings
trim():->removes white space from both the sides of a string
split():-> a string can be converted to an array using this method.

var txt:"a,b,c,d,e";//string

console.log(txt.split(","));//split on comma

console.log(txt.split(" "));//split on space

console.log(txt.split("|"));// split on pipe



========================Date and time in js===================================


Date Methods (get and set)
Time Methods (get and set)

A JavaScript date is fundamentally specified as the number of milliseconds that have elapsed since the ECMAScript epoch, which is defined as January 1, 1970, UTC (equivalent to the UNIX epoch).


creating date objects 4 ways:

new Date();
new Date(year,month,day,hours,minutes,seconds,milliseconds)

new Date(milliseconds);

new Date(dateString);


console.log(new Date());

console.log(new Date().toLocaleString());

console.log(new Date().toString());

Date.now();

new Date(milliseconds);

//Dates methods:

// how to get individual date

const currDate=new Date();

console.log(currDate.getDate());
console.log(currDate.getDay());
console.log(currDate.getFullYear());
console.log(currDate.getHours());
console.log(currDate.getMinutes());
console.log(currDate.getUTCMilliseconds());
console.log(currDate.getMilliseconds());
console.log(currDate.getTime());
console.log(currDate.getTimezoneOffset());
console.log(currDate.getMonth());//0-11 jan-dec

output:

2
3
2022
11
37
690
690
1667374650690
-240
10

//how to set individual date

console.log(currDate.setDate());
console.log(currDate.setDay());
console.log(currDate.setFullYear());
console.log(currDate.setHours());
console.log(currDate.setMinutes());
console.log(currDate.setUTCMilliseconds());
console.log(currDate.setMilliseconds());
console.log(currDate.setTime());
console.log(currDate.setTimezoneOffset());
console.log(currDate.setMonth());//0-11 jan-dec


//how to get individual time 

//how to set individual time


challenge 12:

(8:46:00 before need to do that )

//Math Object in JS 


js math object allows you to perform mathematical tasks on numbers


Math.PI
Math.round()
Math.pow()
Math.sqrt()
Math.abs()
Math.ceil()
Math.floor()
Math.random()
random(): number
Returns a pseudorandom number between 0 and 1.
Math.trunc()returns iintegdr part of number


If the argument is a positive number Math.trunc() is equivalent to Math.floor(),else equal to Math.ceil()




==================================================                             DOM in JS


Window vs Document

Window                                           Document

1.Window is the main container or       1.where document is the                                               child of window object.
we can say the global object and 
any operations related to entire 
browser window can be a part of 
window object.

2.all the members like objects,methods  2.Where in the dom we need                                           to refer the document 
or properties if they are part of window
object then we do not refer to it.


3.window has methods properties and object.3.it is just object of                                                window which deals with html elements
ex:setTimeout()or setInterval() are the 
methods where as document is the object
of window and it also has a screen object 
with proerties of describing physical display.




// difference between DOM vs BOM




BOM:

The BOM is the window object that represents a window in the browser. An object of the window is created automatically by the browser.

The power of the BOM
With the window object, you can:

Manipulate the browser window with the window object and things like scrolling, opening a new window, closing the current window, ..Etc.
Use the object document property to interact with the DOM.
Get the browser history with the history object.
Manipulate the screen with the screen object.
Get and do things with the location object.



DOM:


The DOM (Document Object Model)
DOM = The whole content of the web page

The DOM consists of the document node which represents the content of the page. You can manipulate it using javascript.

The document object represents the whole HTML document. When an HTML document is loaded in the browser, it becomes a document object, and you can use document object to manipulate the web page.

The power of the DOM
There are a lot of things we can do with the DOM object. You’ll be able to pick an HTML element and manipulate it in your JS script.

Change an element text.
Change an HTML element color.
Hide and show elements
Make an HTML elements listen to an event
And much more…
Now that you can differentiate between the BOM and the DOM. Let’s manipulate the web page in the next article by learning how to select HTML elements.


////////////////////////////////////////////////////////OOPs In JS/////////////////////////////////////////

=>Object Literal
=>this in js
object literal:object is simply a key:value data structure

storing variable and functions together in one container.

How to create objects?

//first way of creating object

// let bioData={

//   myname:"maithili",
//   myAge:"26",
//   getData:function(){
//   console.log(`my name is ${bioData.myname}`)
//   }

//   }

// bioData.getData()

//second way of creating object

// let bioData={

//   myname:"maithili",
//   myAge:"26",
//   getData(){
//   console.log(`my name is ${bioData.myname}`)
//   }

//   }

// bioData.getData()

//object inside object

let bioData = {
  myname: {
    firstname: 'maithili',
    lastname: 'kammila',
  },
  myAge: '26',
  getData() {
    console.log(`my name is ${bioData.myname}`);
  },
};

bioData.getData();

//this object in javascript



the definition of "this " object is that it contain the current context.
this object can have different values based on where it is placed.


e.g:


//examples of this

//1.
//console.log(this);
//2

// function myName() {
//   console.log(this);
// }

//myName();

//3

// var name = 'maithili';

// function myName() {
//   console.log(this.name);
// }

// myName();

//4

// let obj = {
//   myage: 26,
//   myname() {
//     console.log(this.myage);
//   },
// };
// obj.myname();

//5(this type can be the interview question)

// let obj={
//   myage:26,
//   myname:()=>{
//     console.log(this.myage);
//   }
// }
// obj.myname();

//as we have learnt arrowfunction does not accept this.

//it will come as undefined.

//what will be the output of this below code?

let bioData = {
  myname: {
    realname: 'maithili',
    channelname: 'myra vlogs',
  },
  myage: 26,
  getBioData() {
    console.log(
      `my name is ${this.myname.channelname} and my age is ${this.myage}`
    );
  },
};

bioData.getBioData();

//ouput:my name is myra vlogs and my age is 26



Destructuring in ES6:

Array destructuring 

Object destructuring


 //ARRAY DESTRUCTURING :

//DEFINITION: array destructuring syntax is an expression that makes it possible unpack values from an arrays or propeties from ojects into distinct variables.

let bioData = ['maithili', 'angajala', 26];

// if we break the array and we wish to assign it to a variable we do like this.

// let fname=bioData[0];
// let lname=bioData[1];
// let age=bioData[2];

// console.log(fname,lname,age);

// now if the array is large we cant do it like one by one so the solution to this is array destructuring, no we do like below

// let [fname,lname,age]=bioData;

// console.log(fname,lname,age);

// if you want add new data also you can acheive that

// let [fname,lname,age,degree="Btech"]=bioData;

//  console.log(fname,lname,age,degree);

//output:maithili angajala 26 Btech


// note:Here in destructuring what matters is the array position that matters it should be in the respective position which you want to assign.



OBJECT DESTRUCTURING:


let obj={
  myfname:"maithili",
  mylname:"kammila",
  age:26
}

// let age=obj.age;
// let myfname=obj.myfname;
// let mylname=obj.mylname;



let {myfname,mylname,age,degree="Btech"}=obj;

console.log(age);


//here the construct is the names should be same while assigning as it is object.

Object Properties:

//we can now use Dynamic properties


let myname="vinod";
const myBio={

myName:"maithili"
26:"is my age"
}

console.log(myBio);
 
 output:
 {26: "is my age", myName: "maithili"}

now if you want to give dynamic value then you can write it in square brackets .


let myname="vinod";
const myBio={

[myName]:"maithili"
[20+6]:"is my age"
}

console.log(myBio);


now output is:
{26: "is my age", vinod: "maithili"}
26: "is my age"
vinod: "maithili"



// no need to write key : value if both are same

for e.g:

let myname="maithili k";

let myage=26;

const myBio={
myname:myname,
myage:myage
}

output:{myname: "maithili k", myage: 26}
myage: 26
myname: "maithili k"
<prototype>: Object




=>spread operator
=>rest operator


ES7 features

array.prototype.includes

exponentiation operator


ES8

string padding
Object.entries()
Object.values()


string padding
padStart(length)
padEnd(length)


object.values()

e.g:
const person={
name:"fred",
age:"27"
}

object.values(person);
object.entries(person);

output:




