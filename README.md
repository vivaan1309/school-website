# school-websitehtml, body
{
  height: 100%;
  margin: 0;
}

body
{
background-image: linear-gradient(to right top, #33a0f1, #2591d9, #1882c1, #0a73aa, #006494);
}

.header
{
	color: rgb(150, 152, 238);font-family: 'Yeon Sung';font-size: 45px;letter-spacing: 10px;margin-top: 80px;
}
.header img
{
	width: 80px;margin-left: -15px;
}

.login_div
{
	background: rgba(235, 36, 36, 0.8);float: none;border-radius: 15px;
}

.logo
{
	width: 80px;margin-top: 30px;border-radius: 40px;
}

#login_button
{
	width: 80%;border-radius: 15px;
}

.room_name
{
	cursor: pointer;
	font-size: 20px;
}


#logout
{
	font-size: 20px; float: right;
}


#output
{
	padding: 10px; width:80%;background: rgba(255,255,255,0.8);border-radius: 15px;
}

.input_div_room_page
{
	width: 80%;
}

.input_div label
{
	color: white;font-size: 20px;
}


.input_div_message_page
{
	position: fixed;bottom: 0px;width: 100%;background: rgba(255,255,255,0.8);
}
.input_div_message_page label
{
	color: black;
}
.input_div_message_page #msg
{
	width: 80%;
}
.input_div_message_page button
{
	margin-top: 15px;
	width: 50%; 
}
.color_white
{
	color: white
}

.user_tick
{
	width:20px;
}
.message_h4
{
	padding-left:5px;color:grey;
}
function addUser() {
    user_name=document.getElementById("user_name").value;
    localStorage.setItem("user_name", user_name);
    window.location="kwitter_room.html";
    
    }






<!DOCTYPE html>
<html>
<head>
	<title>Kwitter</title>
<link href="https://fonts.googleapis.com/css?family=Yeon+Sung&display=swap" rel="stylesheet"><meta name="viewport" content="width=device-width, initial-scale=1">

<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/css/bootstrap.min.css">
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.0/js/bootstrap.min.js"></script>

<link rel="stylesheet" type="text/css" href="kwitter.css">
<script src="kwitter.js"></script>
</head>

<body>
    <center>
        <h1 class="header">	
            Kwitter	<sup>
        <img src="m2.png">
        </sup>
    </h1>
        <div class="col-lg-4 col-md-6 col-sm-6 col-xs-11 login_div">
        <img src="logo.png" class="logo">
            <h3 > Get updated with the school</h3>
            <h4 >Join Kwitter today</h4>
            <div class="form-group">
              <label >User Name:</label>
              <input type="text" id="user_name" class="form-control" placeholder="User Name">
            </div>

            <button id="login_button" class="btn btn-primary" onclick="addUser()"> Log in</button>
            <br>
            <br>
        </div>
    </center>
    </body>
    </html>
