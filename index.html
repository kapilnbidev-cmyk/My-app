<!DOCTYPE html>
<html lang="hi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Video Star</title>

<style>
*{box-sizing:border-box}
body{
 margin:0;
 background:#080b2d;
 color:white;
 font-family:Arial,sans-serif;
}
header{
 padding:22px;
 text-align:center;
 background:linear-gradient(90deg,#7516a8,#ff168d);
}
.logo{font-size:34px;font-weight:bold}
.logo span{color:#ff72c0}
.tag{margin-top:6px;font-size:18px}
.app{max-width:500px;margin:auto;min-height:100vh}
.page{padding:20px}
.card{
 background:#191d49;
 border-radius:20px;
 padding:28px;
}
h1{margin-top:0}
input{
 width:100%;
 padding:15px;
 margin:8px 0;
 border-radius:14px;
 border:1px solid #777;
 background:#0e1235;
 color:white;
 font-size:16px;
}
button{
 width:100%;
 padding:15px;
 margin-top:12px;
 border:0;
 border-radius:28px;
 font-size:17px;
 font-weight:bold;
}
.primary{
 background:linear-gradient(90deg,#ff168d,#a72cff);
 color:white;
}
.link{
 background:none;
 color:#ff72c0;
}
.hidden{display:none}
.message{
 margin-top:12px;
 padding:10px;
 border-radius:10px;
 background:#292e60;
}
nav{
 position:fixed;
 bottom:0;
 left:50%;
 transform:translateX(-50%);
 width:100%;
 max-width:500px;
 display:flex;
 justify-content:space-around;
 background:#111536;
 padding:14px 5px;
}
nav button{
 background:none;
 color:white;
 margin:0;
 padding:5px;
 font-size:14px;
}
</style>
</head>

<body>

<div class="app">

<header>
 <div class="logo">⭐ Video <span>Star</span></div>
 <div class="tag">हर Talent को मिले पहचान</div>
</header>

<div class="page">

<!-- LOGIN -->
<section id="loginPage">
<div class="card">
<h1>Welcome to Video Star 👋</h1>
<p>अपने अकाउंट में Login करें</p>

<input id="loginEmail" type="email" placeholder="Email">
<input id="loginPassword" type="password" placeholder="Password">

<button class="primary" onclick="login()">Login</button>

<button class="link" onclick="showRegister()">
Create New Account
</button>

<div id="loginMsg" class="message hidden"></div>
</div>
</section>

<!-- REGISTER -->
<section id="registerPage" class="hidden">
<div class="card">
<h1>Create New Account 🎉</h1>

<input id="regName" placeholder="आपका नाम">
<input id="regEmail" type="email" placeholder="Email">
<input id="regPassword" type="password" placeholder="Password">

<button class="primary" onclick="register()">
Create Account
</button>

<button class="link" onclick="showLogin()">
Already have an account? Login
</button>

<div id="registerMsg" class="message hidden"></div>
</div>
</section>

<!-- HOME -->
<section id="homePage" class="hidden">
<div class="card">
<h1>Welcome to Video Star 👋</h1>
<h2 id="welcomeName"></h2>
<p>अपनी वीडियो बनाएं, शेयर करें और अपना Talent दिखाएं।</p>
<button class="primary" onclick="logout()">Logout</button>
</div>
</section>

<!-- PROFILE -->
<section id="profilePage" class="hidden">
<div class="card">
<h1>My Profile 👤</h1>
<p><b>नाम:</b> <span id="profileName"></span></p>
<p><b>Email:</b> <span id="profileEmail"></span></p>
<button class="primary" onclick="logout()">Logout</button>
</div>
</section>

</div>

<nav id="nav" class="hidden">
<button onclick="showHome()">🏠<br>Home</button>
<button onclick="showUpload()">➕<br>Upload</button>
<button onclick="showEarnings()">💰<br>Earnings</button>
<button onclick="showProfile()">👤<br>Profile</button>
</nav>

</div>

<script>

function getUsers(){
 return JSON.parse(localStorage.getItem("videoStarUsers") || "[]");
}

function saveUsers(users){
 localStorage.setItem("videoStarUsers",JSON.stringify(users));
}

function showRegister(){
 document.getElementById("loginPage").classList.add("hidden");
 document.getElementById("registerPage").classList.remove("hidden");
}

function showLogin(){
 document.getElementById("registerPage").classList.add("hidden");
 document.getElementById("loginPage").classList.remove("hidden");
}

function register(){

 const name=document.getElementById("regName").value.trim();
 const email=document.getElementById("regEmail").value.trim().toLowerCase();
 const password=document.getElementById("regPassword").value;

 const msg=document.getElementById("registerMsg");
 msg.classList.remove("hidden");

 if(!name || !email || !password){
   msg.innerText="सभी जानकारी भरें।";
   return;
 }

 if(password.length < 6){
   msg.innerText="Password कम से कम 6 अक्षर का रखें।";
   return;
 }

 const users=getUsers();

 if(users.some(u=>u.email===email)){
   msg.innerText="यह Email पहले से मौजूद है। Login करें।";
   return;
 }

 users.push({
   name:name,
   email:email,
   password:password
 });

 saveUsers(users);

 msg.innerText="Account बन गया! अब Login करें।";

 setTimeout(showLogin,800);
}

function login(){

 const email=document.getElementById("loginEmail").value.trim().toLowerCase();
 const password=document.getElementById("loginPassword").value;

 const msg=document.getElementById("loginMsg");
 msg.classList.remove("hidden");

 const users=getUsers();

 const user=users.find(
   u=>u.email===email && u.password===password
 );

 if(!user){
   msg.innerText="Email या Password गलत है।";
   return;
 }

 localStorage.setItem("videoStarCurrentUser",JSON.stringify(user));

 showHome();
}

function showHome(){

 const user=JSON.parse(
   localStorage.getItem("videoStarCurrentUser")
 );

 if(!user){
   showLogin();
   return;
 }

 document.getElementById("loginPage").classList.add("hidden");
 document.getElementById("registerPage").classList.add("hidden");
 document.getElementById("profilePage").classList.add("hidden");
 document.getElementById("homePage").classList.remove("hidden");

 document.getElementById("welcomeName").innerText=
   "नमस्ते, "+user.name+"!";

 document.getElementById("nav").classList.remove("hidden");
}

function showProfile(){

 const user=JSON.parse(
   localStorage.getItem("videoStarCurrentUser")
 );

 if(!user)return;

 document.getElementById("homePage").classList.add("hidden");
 document.getElementById("profilePage").classList.remove("hidden");

 document.getElementById("profileName").innerText=user.name;
 document.getElementById("profileEmail").innerText=user.email;
}

function showUpload(){
 alert("Upload feature अगला चरण है।");
}

function showEarnings(){
 alert("Earnings feature अगला चरण है।");
}

function logout(){

 localStorage.removeItem("videoStarCurrentUser");

 document.getElementById("nav").classList.add("hidden");
 document.getElementById("homePage").classList.add("hidden");
 document.getElementById("profilePage").classList.add("hidden");

 showLogin();
}

window.onload=function(){

 const current=localStorage.getItem("videoStarCurrentUser");

 if(current){
   showHome();
 }else{
   showLogin();
 }

};

</script>

</body>
</html>
