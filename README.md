<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Vivi x Gloo Forever</title>

<style>
body{
margin:0;
padding:0;
height:100vh;
display:flex;
justify-content:center;
align-items:center;
background:linear-gradient(-45deg,#10002b,#240046,#3c096c,#5a189a);
background-size:400% 400%;
animation:bgMove 12s ease infinite;
font-family:Arial, sans-serif;
color:white;
text-align:center;
overflow:hidden;
}

@keyframes bgMove{
0%{background-position:0% 50%;}
50%{background-position:100% 50%;}
100%{background-position:0% 50%;}
}

.container{
z-index:2;
padding:20px;
max-width:400px;
}

h1{
font-size:24px;
margin-bottom:30px;
transition:0.3s;
text-shadow:0 0 10px rgba(255,255,255,0.4);
}

/* Buttons */
button{
padding:14px 30px;
font-size:16px;
border:none;
border-radius:40px;
cursor:pointer;
margin:10px;
transition:0.3s;
}

#yesBtn{
background:linear-gradient(45deg,#ffd60a,#ffea00);
color:black;
box-shadow:0 0 15px gold;
}

#yesBtn:hover{
box-shadow:0 0 25px gold;
transform:scale(1.05);
}

#noBtn{
background:#2d006e;
color:white;
position:relative;
box-shadow:0 0 10px #9d4edd;
}

/* Medal popup */
.medal{
position:absolute;
top:50%;
left:50%;
transform:translate(-50%,-50%) scale(0);
font-size:32px;
font-weight:bold;
color:#ffd60a;
text-shadow:0 0 20px gold;
animation:medalPop 1.2s forwards;
}

@keyframes medalPop{
0%{transform:translate(-50%,-50%) scale(0);opacity:0;}
50%{transform:translate(-50%,-50%) scale(1.6);opacity:1;}
100%{transform:translate(-50%,-50%) scale(1);opacity:0;}
}

/* Mythic banner*
