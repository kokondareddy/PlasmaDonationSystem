<!DOCTYPE html>
<html>
<head>
<title>Home Page</title>
<link rel='stylesheet' href='Home-Style.css'>
</head>
<body>
<nav class="nav">
<div class="logo">
<h1>Plasma Donation</h1>
</div>
<ul class="nav-links">
<li><a href='#' style="color: rgb(59, 172, 182);"> HOME </a></li>
<li><a href="About-Us.html"> ABOUT </a></li>
<li><a href="login-page.html"> LOGIN </a></li>
<li><a href="Registration.html"> SIGNIN </a></li>
</ul>
</nav>
<div class="hero">
<div class="form_box">
<div class="button_box">
<!-- <div id="btn"></div> -->
<button type="button"
class="toggle_btn">CHECK&nbsp;YOUR&nbsp;MATCH!</button>
</div>
<form class="input-group" action="DonorDetails" method="get">
<input type="text" id="input-field" placeholder="Name:">
<input
type="tel" id="input-field" placeholder="Phone number:">
<div class="input-container-hospital">
<!-- <label for="hospital"><b>Hospital</b></label> -->
<input type="text" placeholder="Enter hospital"
list="hospital"
name="hospital" id="input-field">
<datalist id="hospital">
<option value="KAMINENI">
<option value="APOLLO">
<option value="OWAISI">
`15
<option value="CONTINENTAL">
<option value="PRATHIMA">
</datalist>
</div>
<div class="input-container-blood">
<!-- <label for="Blood-Group"><b>Blood Group</b></label> -
->
<input type="text" placeholder="Enter Blood Group"
list="Blood-Group" name="bloodGroup" id="input-field"
required>
<datalist id="Blood-Group">
<option value="A+">
<option value="A-">
<option value="B+">
<option value="B-">
<option value="AB+">
<option value="AB-">
<option value="O+">
<option value="O-">
<option value="Bombay Blood Group">
</datalist>
</div>
<button type="Submit" class="submit-btn">SEARCH</button>
</form>
</div>
<div id="links">
<a href="login-page.html"><p id="link1">I AM A DONOR!</p></a> <a
href="Registration.html"><p id="link2">WANNA BE A
DONOR?</p></a>
</div>
</div>
</body>
</html>
Login Page:
<html>
<head>
<title>login page</title>
<style>
.everything{
margin-top:30px;
margin-left: 40px;
margin-right: 40px;
margin-bottom: 40px;
display: flex;
align-items: center;
justify-content: center;
}
.img{
width:100%;
height:100%;
position: absolute;
}
.loginbox{
height:420px;
background:rgb(176,196,222);
width:340px;
top: 50%;
left: 18%;
border-radius: 2rem;
position:absolute;
transform:translate(-50%,-50%);
box-sizing:border-box;
padding:70px 30px;
}
.user{
height:100px;
width:100px;
border-radius:50%;
position:absolute;
top:-50px;
left:calc(50% - 50px);
}
h1{
margin: 0;
padding: 0 0 20px;
text-align:center;
font-size:22px;
font-weight:bold;
}
.loginbox input{
display: block;
  font-size: 0.675rem;
}
.Sign-up-button{
width:30%;
margin-left:95px;
margin-top:8px;
height:25px;
color:white;
border-radius: 2rem;
border:solid;
border-width: 2px;
border-radius: 2rem;
}
.Sign-up-button:hover{
cursor:pointer;
}
.loginbox a{
margin-left: 70px;
font-size: 16px;
}
.loginbox a:hover{
color: rgb(47, 143, 157);
}
nav{
display: fixed;
top: 0;
width: 100%;
display: flex;
justify-content: space-around;
align-items: center;
max-height: 7vh;
background-color: linear-gradient(rgb(59, 172, 182),rgb(130, 219,
216));
font-family: "Whitney" , sans-serif;
border-bottom: solid;
border-bottom-color: rgb(243, 243, 243);
}
.logo{
margin-top: 19px;
color: rgb(47, 143, 157);
text-transform: uppercase;
letter-spacing: 2.4px;
font-size: 15px;
}
.nav-links{
display: flex;
`18
justify-content: space-around;
width: 30%;
}
.nav-links li{
list-style: none;
}
.nav-links a{
color: black;
text-decoration: none;
letter-spacing: 3px;
font-weight: bold;
font-size: 14px;
border-bottom: 3px solid transparent;
}
.nav-links a:hover{
color: rgb(47, 143, 157);
}
width: 100%;
max-width: 280px;
box-sizing: border-box;
border-radius: 4px;
border:1px solid #c4c4c4;
padding: 1em;
margin-bottom:0.20rem;
</style>
</head>
<body>
<nav>
<div class="logo">
<h1> PLASMA DONATION </h1>
</div>
<ul class="nav-links">
<li> <a href="Home.html" > HOME </a> </li>
<li> <a href="About-Us.html" > ABOUT </a> </li>
<li> <a href="#" style = "color: rgb(47, 143, 157);"> LOGIN </a>
</li>
<li> <a href="Registration.html" > SIGNIN </a> </li>
</ul>
</nav>
<div class="everything" >
<div class ="split-screen">
<div class="loginbox">
<img src="pds images\149071.png" class="user">
<h1>LOGIN HERE</h1>
<form action = "ModifyPage" method = "get">
<strong>Email-ID</strong><br/>
<input type="text" name="email" placeholder="Enter Email-ID">
<br>
<strong>Password</strong><br/>
<input type="password" name="password" placeholder="Enter
Password">
<br>
`19
<button class="Sign-up-button"
type="submit">Login</button>
<br>
<br>
<a href="ForgotPassword.html" style="margin-left:80px;">Forgot
Password?</a>
<br>
<br>
<a href="Registration.html" style="margin-left:65px;">Don't
have an account?</a>
</div>
<div class="img"><img src="pds images\Plasma.png" alt="HTML5 Icon"
width="600" height="600"></div>
</div>
</div>
</body>
</html>
Registration Page:
<!DOCTYPE html>
<html>
<head>
<title>Registration</title>
<script
src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></scrip
t>
<script>
// Function to check Whether both passwords
// is same or not.
function checkPassword(form) {
password = form.password.value;
password2 = form.password2.value;
// If password not entered
if (password == '')
alert ("Please enter Password");
// If confirm password not entered
else if (password2 == '')
alert ("Please enter confirm password");
// If Not same return False.
else if (password != password2) {
`20
alert ("\nPassword did not match: Please enter again.")
return false;
}
// If same return TTrue.
else{
return true;
}
}
function myfun(){
var a=document.getElementById("Phoneno.").value;
var msg = document.getElementById("msg");
if(a==""){
msg.innerHTML= "**Please fill the column";
}
else if(isNaN(a)){
msg.innerHTML = "**only numeric values allowed";
}
else if(a.length<10){
msg.innerHTML = "**invalid number";
}
else if(a.length>10){
msg.innerHTML = "**invalid number";
}
// else{
// return true;
// }
}
</script>
<link rel='stylesheet' href='Registration-Style.css'>
</head>
<body>
<nav>
<div class="logo" >
<h1 style="letter-spacing: 2.2px;
font-size: 23px;"> PLASMA DONATION </h1>
</div>
<ul class="nav-links">
<li> <a href="Home.html" > HOME </a> </li>
<li> <a href="About-Us.html" > ABOUT </a> </li>
<li> <a href="login-page.html" > LOGIN </a> </li>
<li> <a href="#" style = "color: black"> SIGNIN </a> </li>
</ul>
</nav>
<div class = "everything">
<div class ="split-screen">
<div class="left-screen">
<img src="pds images\home1.jpg" width="500" height="500">
<!-- <section class="copy">
<h1>Donate Plasma</h1>
<h1>Save lives</h1>
</section> -->
</div>
<div class="right-screen">
<form onsubmit="return checkPassword(this)" action =
"UserRegistration" method = "get" >
<section class="copy">
<h2>Sign Up</h2>
<div class="login-form">
<p>Already have an account? <a
href="#"><strong>Log In</strong></a></p>
</div>
</section>
<div class="container">
<div class="container-left">
<div class="input-container name">
<label for="Name"><b>Name</b></label>
<input type="text" placeholder="Enter Name"
name="uname" id="Name" required>
</div>
<div class="input-container email">
<label for="email"><b>Email</b></label>
<input type="email" placeholder="Enter Email"
name="email" id="email" required>
</div>
<div class="input-container Phone Number">
<label for="Phoneno."><b>Phone
Number</b></label>
<input type="tel" placeholder="Enter Phone
Number" name="mobilNo" id="Phoneno." required>
<p id="msg" style="color:rgb(82, 94, 117)">
</p>
</div>
<div class="input-container Address">
<label for="Address"><b>Address</b></label>
<input type="text" placeholder="Enter Address"
name="address" id="Address" required>
</div>
<div class="input-container Pincode">
<label for="Pincode"><b>Pincode</b></label>
<input type="text" placeholder="Enter Pincode"
name="pincode" id="Pincode" required>
</div>
</div>
<div class="container-right">
`22
<div class="input-container DOB">
<label for="DOB"><b>DOB</b></label>
<input type="date" placeholder="Enter DOB"
name="dob" id="DOB"
required>
</div>
<div class="input-container-Gender">
<lable style="display: flex ;font-size:
17px;margin-bottom: 0.5rem;margin-top:0.5rem"><b>Gender</b></lable>
<input type="radio" name="gender" id="male"
value="Male">
<label for="male" style="float: left"
>Male</label>
<input type="radio" name="gender" id="female"
value="Female">
<label for="female" style="float: left"
>Female</label>
<input type="radio" name="gender" id="others"
value="Others">
<label for="others" style="float: left ;
padding-bottom: 2px" >Others</label>
</div>
<div class="input-container-blood">
<label for="Blood-Group"><b>Blood
Group</b></label>
<input type="text" placeholder="Enter Blood
Group" list="Blood-Group" name="bloodGroup" required>
<datalist id="Blood-Group">
<option value="A+">
<option value="A-">
<option value="B+">
<option value="B-">
<option value="AB+">
<option value="AB-">
<option value="O+">
<option value="O-">
<option value="Bombay Blood Group">
</datalist>
</div>
<div class="input-container Password">
<label for="password"><b>Password</b></label>
`23
<input type="password" placeholder="Enter
password" name="password" id="password" required>
<i class=" for fa-eye-slash"></i>
</div>
<div class="input-container Confirm">
<label for="conform"><b>Confirm
Password</b></label>
<input type="password" placeholder="Confirm
password" name="password2" id="confirm password" required>
</div>
</div>
</div>
<div class="input-container-health">
<label class="checkbox-container">
<input type="checkbox">
Yes, I have no health issues.
</label>
</div>
<button class="Sign-up-button"
type="submit" onclick="myfun()">Sign Up</button>
</form>
</div>
</div>
</div>
</body>
</html>
