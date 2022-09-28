1) contact.xhtml

<?xml version = "1.0" encoding = "utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">

<html xmlns="http://www.w3.org/1999/xhtml">
	<head>
		<title>MCA Department</title>
	</head>
	<body bgcolor="AliceBlue">
		<h1 align="center"> CMR INSTITUTE OF TECHOLOGY</h1>
		<h2 align="center"> MCA DEPARTMENT</h2>
		<p>
			<a href="home.xhtml">Home</a>
		</p><hr/>
		<center><p>
		<strong>Address</strong>
		CMR Institute of Technology<br/>
		132 AECS Layout<br/>
		ITPL Main Road<br/>
		Kundalahalli<br/>
		Bangalore 560037, India<br/>
		</p>
		<p>
		<strong>Call:</strong>
		+91 80 28524466 / 77
		<strong>Email:</strong>
		info@cmrit.ac.in
		</p>
		<p>
		<strong>Office hours:</strong>
		8.00 am to 4.00 pm (Monday – Friday)<br/>
		8.00 am to 12.30 pm (Saturday)	
		</p>
		</center>
	</body>
</html>

home.xhtml=


<?xml version = "1.0" encoding = "utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">

<html xmlns="http://www.w3.org/1999/xhtml">
	<head>
		<title>MCA Department</title>
	</head>
	<body bgcolor="AliceBlue">
		<h1 align="center"> CMR INSTITUTE OF TECHOLOGY</h1>
		<h2 align="center"> MCA DEPARTMENT</h2>
		<p>
			<a href="#1">Overview</a>&nbsp;&nbsp;&nbsp;
			<a href="#2">Faculty</a> &nbsp;&nbsp;&nbsp;
			<a href="#3">Time Table</a> &nbsp;&nbsp;&nbsp;
			<a href="contact.xhtml">Contact</a> &nbsp;&nbsp;&nbsp;
		</p><br/>
		<img src="2.jpg"  alt="image" width="100%" height="300px"/><br/>
		
		<h3 id="1" style="color: maroon;">Department Overview</h3>
		<p> The Department of MCA was established in 2001. 
			The Department offers a postgraduate degree titled ‘Master of Computer Applications’. 
			The programme is of 3 years (6 semesters) duration. The current student intake for the programme is 120.</p><br/>
		<hr/><br/>
		<h3 id="2">Faculty</h3>
		<pre>
		
			Ms.Gomathi | Head of Department 		Ms. Moumita Roy | Assistant Professor 		Ms. Uma B | Assistant Professor 
		
			Ms. Helen J | Assistant Professor 		Ms. Neha Agrawal | Assistant Professor 		Ms. Aswini Patil | Assistant Professo
		</pre><br/>
		<hr/><br/>
		<h3 id="3">Time Table</h3>
		<table border="1" cellspacing="5" cellpadding="5">
			<tr>
			<td></td>
			<td>8-9</td>
			<td>9-10</td>
			<td>10-10:30</td>
			<td>10.30-11.30</td>
			<td>11.30-12:30</td>
			<td>12:30-1:30</td>
			<td>1:30-2:30</td>
			<td>2:30-3:30</td>
			</tr>
			<tr>
				<td>Day 1</td>
				<td>web</td>
				<td>unix</td>
				<td rowspan="3">Break</td>
				<td>dms</td>
				<td>co</td>
				<td rowspan="3">Break</td>
				<td>ds</td>
				<td>unix</td>
			</tr>
			<tr>
				<td>Day 2</td>
				<td>web</td>
				<td>unix</td>
				
				<td>dms</td>
				<td>co</td>
				
				<td>ds</td>
				<td>unix</td>
			</tr>
			<tr>
			<td>Day 3</td>
				<td>web</td>
				<td>unix</td>
				
				<td>dms</td>
				<td>co</td>
				
				<td>ds</td>
				<td>unix</td>
			</tr>
		</table>
	</body>
</html>

2) lab2.xhtml
<?xml version = "1.0" encoding = "utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">

<html xmlns="http://www.w3.org/1999/xhtml">
	<head>
		<title>Program 2</title>
		<link rel="stylesheet" type="text/css" href="mycss.css" />
		<style type="text/css">
			ol{list-style-type:upper-roman;}
			ol ol{list-style-type:upper-alpha;}
			ol ol ol{list-style-type:decimal;}
			ul{list-style-type:square;}
			h3{font-family:'Courier New'; font-size:18pt}
			#two{
			 font-style:italic;
			}
			.one{
				font-weight:bold;
				font-family:'Courier New';
			}
		</style>
	</head>
	<body style="background-color:AliceBlue">
		
		<p class="one" style="margin:0.2in; padding:0.2;background-color:#C0C0C0; border-style:solid;"> The Department of MCA was established in 2001. 
			The Department offers a postgraduate degree titled ‘Master of Computer Applications’. 
			The programme is of 3 years (6 semesters) duration. The current student intake for the programme is 120.</p>
		<p id="two" style="margin:0.1in; padding:0.3;background-color:#C0C0C0; border-style:solid;"> The Department of MCA was established in 2001. 
			The Department offers a postgraduate degree titled ‘Master of Computer Applications’. 
			The programme is of 3 years (6 semesters) duration. The current student intake for the programme is 120.</p>
		<p style="margin:0.3in; padding:0.1;background-color:#C0C0C0; border-style:solid;"> The Department of MCA was established in 2001. 
			The Department offers a postgraduate degree titled ‘Master of Computer Applications’. 
			The programme is of 3 years (6 semesters) duration. The current student intake for the programme is 120.</p>
		
		<h2>Aircraft Type</h2>
		<ol>
			<li>General Aviation
				<ol>
					<li>Single Engine Aircraft
						<ol>
							<li>Tail wheel</li>
							<li>Tricycle</li>
						</ol>
					</li>
					<li>Dual Engine Aircraft
						<ol>
							<li>Wing-mounted engines</li>
							<li>Push-pull fuselage-mounted engines</li>
						</ol>
					</li>
				</ol>
			</li>
		</ol>
		
		<h3>Common single-engine aircraft</h3>
		<ul>
			<li>Cessna Skyhawk</li>
			<li>Beechcraft Bonanza</li>
			<li>Piper Cherokee</li>
		</ul>
		<br/>
		<table border="1">
			<caption>Fruit Juice Drinks</caption>
			<tr>
				<th></th>
				<th>Apple</th>
				<th>Orange</th>
				<th>Watermelon</th>
			</tr>
			<tr>
				<th>Breakfast</th>
				<td>0</td>
				<td>1</td>
				<td>0</td>
			</tr>
			<tr>
				<th>Lunch</th>
				<td>1</td>
				<td>0</td>
				<td>0</td>
			</tr>
			<tr>
				<th>Dinner</th>
				<td>0</td>
				<td>0</td>
				<td>1</td>
			</tr>
		</table>
	</body>
</html>

my stle.css-

body{
	background-color:red;
}
table,th{
				border-top-width:medium;
				border-top-color:red;
				border-top-style:dashed;
				border-bottom-width:thick;
				border-bottom-color:blue;
				border-bottom-style:dotted;
			}
p{
	font-family:'Arial'
}

3)a) <!DOCTYPE html>  
<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Lab3a</title>
	</head>
    <body>
        <script type="text/javascript">
            //initialize variables
            var fib1=0,fib2=1,fib=0;
            var n=prompt("Enter a number");
            if(n!=null && n>0)
                {
                    document.write("<h1>First " + n + " Fibonacci numbers are: </h1><br>");
                    //if input is one number
                    if(n==1)
                     document.write("<p>" + fib1 + "</p><br/>");
                    //if input is two numbers
                    else
                        document.write("<p>" + fib1 + "</p><br/><p>" + fib2 + "</p><br/>");
                        //if input is more than two numbers, find the next Fibonacci number
                        for(i=3;i<=n;i++)
                            {
                                fib=fib1+fib2;
                                document.write("<p>" + fib + "</p><br/>");
                                fib1=fib2;
                                fib2=fib;
                            }
                }
            else
                alert("Please enter proper input value");
        </script>
    </body>
 </html>
 
 3)a)
 <!DOCTYPE html>  
<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Lab3a</title>
	</head>
    <body>
        <script type="text/javascript">
            //initialize variables
            var fib1=0,fib2=1,fib=0;
            var n=prompt("Enter a number");
            if(n!=null && n>0)
                {
                    document.write("<h1>First " + n + " Fibonacci numbers are: </h1><br>");
                    //if input is one number
                    if(n==1)
                     document.write("<p>" + fib1 + "</p><br/>");
                    //if input is two numbers
                    else
                        document.write("<p>" + fib1 + "</p><br/><p>" + fib2 + "</p><br/>");
                        //if input is more than two numbers, find the next Fibonacci number
                        for(i=3;i<=n;i++)
                            {
                                fib=fib1+fib2;
                                document.write("<p>" + fib + "</p><br/>");
                                fib1=fib2;
                                fib2=fib;
                            }
                }
            else
                alert("Please enter proper input value");
        </script>
    </body>
 </html>
 
 3)b)
 
 <!DOCTYPE HTML>
<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Lab3b</title>
		 
	</head>
	 
	<body>
	<h2> Javascript to generate squares of 1 to 'N' numbers</h2>
	<script type="text/javascript">
			
				var n=prompt ("Enter the limit 'n' to generate the table of numbers from 1 to n:","");
				var msg="";
				var res= "0";
				for(var x= 1; x<=n;x++)
				{
					res = x * x;
					msg = msg + " " + x + " * "+ x + " = " + res + "\n";
				}
				alert(msg);
			 
		</script>
	</body>
</html>

4)a)

<!DOCTYPE html>
<html>
	<head>
		<title>Program 4a</title>
		<script type="text/javascript">
			var cost1=0, cost2=0, cost3=0, totcost=0, sale_cost=0;
			function fun1(t1)
			{
				cost1=parseInt(cost1+t1);
			
			}
			function fun2(t2)
			{
				cost2=parseInt(cost2+t2);
				
			}
			function fun3(t3)
			{
				cost3=parseInt(cost3+t3);
				
			}
			function show()
			{
				totcost=parseInt(cost1+cost2+cost3);
				sale_cost=(totcost*0.05);
				totcost=totcost+sale_cost;
				alert("Your total cost is : $"+(totcost));
				return false;
			}
		</script>
	</head>
	<body>
		
		<input type="checkbox" name="check1" value="59" onClick="fun1('59')">Apple 59 cents </br>
		<input type="checkbox" name="check2" value="49" onClick="fun2('49')">Orange 49 cents </br>
		<input type="checkbox" name="check3" value="39" onClick="fun3('39')">Banana 39 cents </br>
		<input type="submit" value="click" name="submit" onClick="show()"/>
	</body>
</html>

4) b)

<!DOCTYPE html>
<html>
	<head>
		<title>Program 4b</title>
		<script type="text/javascript">
			var cost1=0, cost2=0, cost3=0, totcost=0, sale_cost=0;
			function fun1(t1)
			{
				cost1=parseInt(cost1+t1);
			}
			function fun2(t2)
			{
				cost2=parseInt(cost2+t2);
				
			}
			function fun3(t3)
			{
				cost3=parseInt(cost3+t3);
				
			}
			function show()
			{
				var qty1=parseInt(document.getElementById("qty1").value);
				var qty2=parseInt(document.getElementById("qty2").value);
				var qty3=parseInt(document.getElementById("qty3").value);
				if(qty1){
					cost1=parseInt(cost1*qty1);
				}
				if(qty2){
					cost2=parseInt(cost2*qty2);
				}
				if(qty3){
					cost3=parseInt(cost3*qty3);
				}
				totcost=cost1+cost2+cost3;
				sale_cost=Math.round(totcost*0.05);
				totcost=totcost+sale_cost;
				alert("Your total cost is : $"+(totcost));
				return false;
			}
		</script>
	</head>
	<body>
		
		<input type="checkbox" name="check1" value="59" onclick="fun1('59')">Apple 59 cents  Quantity:<input type="text" name="qty1" id="qty1"/></br>
		<input type="checkbox" name="check2" value="49" onclick="fun2('49')">Orange 49 cents Quantity:<input type="text" name="qty2" id="qty2"/></br>
		<input type="checkbox" name="check3" value="39" onclick="fun3('39')">Banana 39 cents Quantity:<input type="text" name="qty3" id="qty3"/></br>
		<input type="submit" value="click" name="submit" onclick="show()" />
	</body>
</html>

5)a)

<!DOCTYPE html>
<html>
	<head>
		<title>Program 5a</title>
		<script type="text/javascript">
			function funValidate(){
				var usn=document.getElementById('usn').value;
				var pattern=/^[1-4]{1}[A-Z]{2}[0-9]{2}[A-Z]{3}[0-9]{2}$/;
				
				if(usn.match(pattern))
				{
					alert("Valid Format");
				}
				else
				{
					alert("Invalid Format");
				}
			}
			
		</script>
	</head>
	<body>
		<label>Enter your USN: <input type="text" name="usn" id="usn" /></label>
		<input type="submit" name="validate" onClick="funValidate()" />
	</body>
</html>

5)b)

<!DOCTYPE html>
<html>
	<head>
		<title>Program 5b</title>
		<script type="text/javascript">
			function funValidate(){
				var usn=document.getElementById('usn').value;
				var sem=document.getElementById('sem').value;
				var usn_pattern=/^[1-4]{1}[A-Z]{2}[0-9]{2}[A-Z]{3}[0-9]{2}$/;
				var sem_pattern=/^[1-6]{1}$/;
				if((usn.match(usn_pattern))&&(sem.match(sem_pattern)))
				{
					alert("Valid Format");
				}
				else if((!usn.match(usn_pattern))&&(sem.match(sem_pattern)))
				{
					alert("Invalid USN and Valid Sem");
				}
				else if((usn.match(usn_pattern))&&(!sem.match(sem_pattern)))
				{
					alert("Valid USN and Invalid Sem");
				}
				else{
					alert("Both are invalid");
				}
			}
			
		</script>
	</head>
	<body>
		<label>Enter your USN: <input type="text" name="usn" id="usn" /></label>
		<label>Enter your Sem: <input type="text" name="sem" id="sem" /></label>
		<input type="submit" name="validate" onClick="funValidate()" />
	</body>
</html>

6)a)

<!DOCTYPE HTML>
<?xml version="1.0" encoding="UTF-8"?>
<html>
<head>
<script type ="text/javascript">
function str_vowel()
{
 var str=prompt("Enter the string\n", " ");
 var pos=str.search(/[aeiou]/i);
 if(pos>=0){
	 document.write("The entered string is:" +str+ "<br/>");
	 document.write("The leftmost vowel is :"+str.charAt(pos)+"<br/>");
	 document.write("The position of the leftmost vowel " +str.charAt(pos), " is:" +(pos+1),"\n");
	 exit;
 }
 else
 {
	 document.write("The entered string is:" +str+ "<br/>");
	 document.write("The entered string has no vowels");
 }
 			
}
</script>
</head>
<body onload = "str_vowel();"> 
</body>
</html>

6)b)

<!DOCTYPE HTML>
<?xml version="1.0" encoding="UTF-8"?>
<html>
<head>
<script type ="text/javascript">
function rev_num()
{
	var num = prompt("Enter the number to be reveresed :", " ");
	var n= num;
	var rev = 0, rem;
	while (n>0)
	{
		rem = n % 10;
		rev = rev * 10 + rem ;
		n = Math.floor(n/10);
	}
	document.write("The given number is : " +num+ " <br/> The reversed number is : " +rev+ "\n");
}
</script>
</head>
<body onload = "rev_num();"> 
</body>
</html>

7)a)

<!DOCTYPE html>  
<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Lab7a</title>
			<style> 
				#Progress_Status { 
				width: 50%; 
				background-color: #ddd; 
				} 

				#myprogressBar { 
				width: 2%; 
				height: 20px; 
				background-color: #4CAF50; 
				} 
			</style>
	</head> 
	<body> 
		<p>Download Status of a File:</p> 
		<div id="Progress_Status"> 
			<div id="myprogressBar"></div> 
		</div> 
		<br/> 
		<button onclick="update()">Start Download</button> 
		<script> 
			function update() { 
			var element = document.getElementById("myprogressBar"); 
			var width = 1; 
			var identity = setInterval(scene, 5); 
			function scene() { 
				if (width >= 100) { 
				clearInterval(identity); 
				} else { 
				width++; 
				element.style.width = width + '%'; 
				} 
			} 
			} 
		</script> 
	</body> 
</html> 

7)b)

<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8">
		<title>Lab7b</title>
	</head>
	<body>
		<video width="500" height="450" controls>
		  <source src="movie.mp4" type="video/mp4">
		  Your browser does not support the video tag.
		</video>
	</body>
</html>

8)a)

<?xml version = "1.0" encoding = "utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
	<head>
		<title>Program 8a</title>
		<script type="text/javascript">
			var oldid="p3";
			function toTop(newid)
			{
				domTop=document.getElementById(oldid).style;
				domNew=document.getElementById(newid).style;
				domTop.zIndex="0";
				domNew.zIndex="10";
				
				oldid=newid;
				
			}
		</script>
		<style type="text/css">
			.para1{
				position:absolute;
				top:0px;
				left:0px;
				z-index:0;
				width:200px;
				height:200px;
				background-color:red;
			}
			.para2{
				position:absolute;
				top:100px;
				left:100px;
				z-index:0;
				width:200px;
				height:200px;
				background-color:blue;
			}
			.para3{
				position:absolute;
				top:200px;
				left:200px;
				z-index:0;
				width:200px;
				height:200px;
				background-color:green;
			}
		</style>
	</head>
	<body>
		<p class="para1" id="p1" onmouseover="toTop('p1')"> Frame One </p>
		<p class="para2" id="p2" onmouseover="toTop('p2')"> Frame Three </p>
		<p class="para3" id="p3" onmouseover="toTop('p3')"> Frame Two </p>
		
		
	</body>
</html>


8)b)

<?xml version = "1.0" encoding = "utf-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN" "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
	<head>
		<title>Program 8b</title>
		<script type="text/javascript">
			var oldid="p3";
			function toTop(topid)
			{
				domTop=document.getElementById(oldid).style;
				domNew=document.getElementById(topid).style;
				domTop.zIndex="0";
				domNew.zIndex="10";
				oldid=topid;
				
			}
			function toDown(downid)
			{
				
				document.getElementById(downid).style.zIndex="0";
				
			}
		</script>
		<style type="text/css">
			.para1{
				position:absolute;
				top:0px;
				left:0px;
				z-index:0;
				width:200px;
				height:200px;
				background-color:red;
			}
			.para2{
				position:absolute;
				top:100px;
				left:100px;
				z-index:0;
				width:200px;
				height:200px;
				background-color:blue;
			}
			.para3{
				position:absolute;
				top:200px;
				left:200px;
				z-index:0;
				width:200px;
				height:200px;
				background-color:green;
			}
		</style>
	</head>
	<body>
		<p class="para1" id="p1" onmouseover="toTop('p1')" onmouseout="toDown('p1')"> Frame One </p>
		<p class="para2" id="p2" onmouseover="toTop('p2')" onmouseout="toDown('p2')"> Frame Three </p>
		<p class="para3" id="p3" onmouseover="toTop('p3')" onmouseout="toDown('p3')"> Frame Two </p>
		
		
	</body>
</html>


9)

<!DOCTYPE html>
<html>
	<head>
		<title>Program 9</title>
		<script type="text/javascript">
			function add(){
				var n1=document.getElementById("num1").value;
				var n2=document.getElementById("num2").value;
				
				var result= parseInt(n1)+parseInt(n2);
				document.getElementById("res").value=result;
			}
			function sub(){
				var n1=document.getElementById("num1").value;
				var n2=document.getElementById("num2").value;
				if((n1=="")||(n2=="")){
					alert("Please enter both the numbers");
					return false;
				}
				var result= parseInt(n1)-parseInt(n2);
				document.getElementById("res").value=result;
			}
			function mul(){
				var n1=document.getElementById("num1").value;
				var n2=document.getElementById("num2").value;
				if((n1=="")||(n2=="")){
					alert("Please enter both the numbers");
					return false;
				}
				var result= parseInt(n1)*parseInt(n2);
				document.getElementById("res").value=result;
			}
			function div(){
				var n1=document.getElementById("num1").value;
				var n2=document.getElementById("num2").value;
				if((n1=="")||(n2=="")){
					alert("Please enter both the numbers");
					return false;
				}
				if(parseInt(n2)>0)
				{
					var result= parseInt(n1)/parseInt(n2);
					document.getElementById("res").value=result;
				}
				else
				{
					document.getElementById("res").value="";
					alert("Divide By Zero");
					return false;
				}
			}
			function clearAll(){
				document.getElementById("num1").value="";
				document.getElementById("num2").value="";
				document.getElementById("res").value="";
			}
			
			
		</script>
	</head>
	<body style="text-align: center;">
		<h1> A SIMPLE CALCULATOR </h1>
		<label>Number 1 = </label><input type="text" id="num1"/><br/><br/>
		<label>Number 2 = </label><input type="text" id="num2"/><br/><br/>
		<label>Result = </label><input type="text" id="res"/><br/><br/>
		<input type="button" value="ADD" onclick="add();"/>
		<input type="button" value="SUB" onclick="sub();"/>
		<input type="button" value="MUL" onclick="mul();"/>
		<input type="button" value="DIV" onclick="div();"/>
		<input type="button" value="CLEAR" onclick="clearAll();"/>
	</body>
</html>

