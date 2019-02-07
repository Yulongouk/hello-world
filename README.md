# Javascript
2.Creating global variable and accessing them
Answer=
 var str="Hello world";
 function clicked()
{
alert(str);
}
<button onclick=clicked()>click</button>
3.create object
 function clicked()
{
 var car={
     no: 123
     name: hello
     }
alert(car.no+car.name);

4.Accessing object properties
objectname.propertyName
or
objectname["propertyName"]
5.Creating object with dynamic values
function clicked()
{
	var name=
	   	{
            first:document.getElementById('one').value,
            last:document.getElementById('two').value,
	   	}
	   	alert(name.first+name.last);
	   }
	<input type="text" id="one" placeholder="Enter the first name of your">
	<input type="text" id="two" placeholder="Enter the last name of your">
   <button onclick="clicked()">click meh</button>
6.Creating method inside objects
<!DOCTYPE html>
<html>
<head>
	<title></title>
	<script type="text/javascript">
	   function getting()
	   {
	   	var name=
	   	{
            first:"Yulong",
            last:"Ouk",
            myname : function()
            {
               return this.first+" "+this.last;
            }
	   	}
	   	alert(name.myname());
	   }
	</script>
</head>
<body>
   <button onclick="getting()">click meh</button>
</body>
</html>
}
7.Passing arguments
<!DOCTYPE html>
<html>
<head>
	<title>passing argument</title>
	<script type="text/javascript">
		function day(myday)
		{
			alert(myday);
		}
	</script>
</head>
<body>
       <button onclick="day('monday')">click</button>
</body>
</html>
8.returning values from functions
#return function in array
	{
			var hello = ["World","My planet"];
			function clicked()
			{
				var newstr= hello.map(me);
				alert(newstr);

			}
			function me(arr)
			{
				var arr= arr+"Earth";
				return arr;
			}
        }
or
return function 
<!DOCTYPE html>
<html>
<body>

<p id="demo"></p>

<script>
function myFunction(name) {
  return "Hello " + name;
}
document.getElementById("demo").innerHTML = myFunction("John");
</script>

</body>
</html>

9.Using function like variable
10.Using event inside function
#Onclick : It reacts when the button is clicked
var str="Hello";
function clicked()
{
alert(str);
}
<button onclick="clicked()">click me</button>
#onmoverover : It reacts when the pointer over the button;
var str="Hello";
function clicked()
{
alert(str);
}
<button onmouseover="clicked()">click me</button>
#Onchange: It occurs when the value of an element has been changed.
Ex:
<!DOCTYPE html>
<html>
<head>
	<title>return value</title>
	<script type="text/javascript">
		{
			function changed()
			{
				var car= document.getElementById("one").value;
				document.getElementById("show").innerHTML="You select"+ car;
			}
        }
	</script>
</head>
<body>
	<p>Choose your choice to get a new one</p>
  <select id="one" onchange="changed()">
  	<option value="BMW" >BMW</option>
  	<option value="Ford">Ford</option>
  	<option value="Toyota">Toyota</option>
  </select>
  <div id="show"></div>
</body>
</html>
11.Array intro
Array is collection of data item store under a common name.
The index value of the first element of array 
always 0.
The index value of the last element of array is length-1
12.Array method
+ toString() use for coverts an array to a string of array values.
+join() is the same as toString() but you can add specify the sperator
+shift() use for remove element at the beginning of array
+unShift() use for add element at the beginning of array
+delete use for deleted the index value
13.Accessing element using index of the array
var fruits = ["Banana", "Orange", "Apple", "Mango"];
var last = fruits[fruits.length-1];
document.getElementById("demo").innerHTML = last;
14.Accessing arrays using forEach
 var arr=[12,23,34,45];
	 function hello()
	 {
	 	arr.forEach(myarr)
	 }
	 function myarr(index)
	 {
	 	alert(index);
	 }
15.Adding more elements into an array
+push()
+pop()
+shift()
+unshift()
16.Associative array
Javascript doesn't support the array with named index.
And Arrays always use the numbered indexes.
Ex= var person =[]
        person[0]= "Jonh"
        person[1]= "Doe"
        person[2]= 46
var x = person.length
var y = person[0]
alert(person[0]+" "+person.length);
17.One dimension array
var Englishteam=["Man city","Liverpool","Man United"]
Two dimension array
var Know=["fruit",["mango","apple","banana"],"meat"];
Muti dimension array
var know=["fruit"["mango"["vitaminA","vitaminB","vitaminC"],"apple","banana"],"meat"];
