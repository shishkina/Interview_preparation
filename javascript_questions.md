#### 1. What is JavaScript?
JavaScript is a scripting language most often used for client-side web development.
#### 2. What is the difference between JavaScript and JScript?
They are similar.
JavaScript was developed by Netscape. Microsoft reverse engineered JavaScript and called in JScript.
#### 3. How to add JavaScript onto a web page?
Two commonly used ways:

1)  short code for a single page, place a ```<script>``` tag inside ```<head>``` element:
```
<head>
<title>Title</title>
<script language="JavaScript" type="text/javascript">
   var name = "Kate Shishkina"
   alert(name);
</script>
</head>
```
2) large code, make a separate ```.js``` file and add its path in the ```<script>```
```
<head>
<title>Title</title>
<script type="text/javascript" src="myjavascript.js"></script>
</head>
```
#### 4. Is JavaScript case sensitive?
Yes. A function getElementById is not the same as getElementbyId
#### 5. What are the types used in JS?
String, Number, Boolean, Function, Object, Null, Undefined
#### 6. What are Boolean operators supported by JavaScript?
And operator: &&  
Or operator: ||
Not operator: !
#### 7. What is the difference between "==" and "==="?
"==" checks equality only
"===" checks foe equality as well as type.
#### 8. How to access the value of a textbox using JS?
We can access the value using ```getElementById``` function.
Example:
```
<!DOCTYPE html>
<html>
<body>
Full name: <input type="text" id="txtFullName"
name="FullName" value="Kate Shishkina">
</body>
</html>
```
```
var name = document.getElementById('txtFullName').value;
alert(name);
```
#### 9. How will you get the ```Checkbox``` status whether checked or not?
```
var status = document.getElementById('checkbox1').checked;
alert(status);
```
will return ```true``` or ```false```
#### 10. If an array with names as "names" contain three elements, then how will you print the third element of this array?
```
document.write(names[2])
```
#### 11. How to submit a form using JS?
```
document.forms[0].submit();
```
#### 12. What does isNaN function do?
It returns ```true``` if the argument is not a number.
#### 13. What is the use of Math Object in JS?
The Math object provides properties and methods for mathematical constants and functions.
#### 14. What do you understand by ```this``` keyword in JS?
In JS ```this``` is a context-pointer and NOT and object pointer.It gives the top-most context that is placed on the stack.
#### 15. What does "1"+2+4 evaluate to?
Since "1" is a string, it is concatenated with the following values.Therefore, the answer is 124.
#### 16. What does 3+4+"7"?
Since 3 and 4 are integers, this is number arithmetic, since "7" is a string, it is concatenation, so the answer is 77.
#### 17. How do you change the style/class on any element using JS?
```
document.getElementById(“myText”).style.fontSize = “10";
```
or
```
document.getElementById(“myText”).className = “anyclass”;
```
#### 18. What looping structures are there in JS?
```for```,```while```, ```do-while``` loops
#### 19. What is an object in JS, give an example?
An object is just a container for a collection of named values.
//Create a cat object.
```
var cat = new Object();
cat.name = "Fluffy";
cat.age = 3;
```
#### 20. How would you add a function as a property in a JS object?
```
cat.getName = function(){
return cat.name;
}
console.log(cat.getName());
