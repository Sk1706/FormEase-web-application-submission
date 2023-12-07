# FormEase-web-application-submission
#html code
<html>
<head>
    <title>How to make website</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    
    <div class="banner">
        <div class="navbar">
            <img src="logo.png" class="logo">
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Bedroom</a></li>
                <li><a href="#">Dining</a></li>
                <li><a href="#">Kitchen</a></li>
                <li><a href="#">Backyard</a></li>
            </ul>
        </div>
        <div class="content">
            <h1>Hey! Glad to see you</h1>
            <p>MY HOUSE<br>"Home is the nicest word there is"</p>
            <div>
                <button type="button"><span></span>WATCH MORE</button>
                <button type="button"><span></span>VIDEOS</button>
            </div>
        
        </div>
    </div>
    
#css code
*{
    margin: 0;
    padding: 0;
    font-family: sans-serif;
}
.banner{
    width: 100%;
    height: 100vh;
    background-image: linear-gradient(rgba(0,0,0,0.75),rgba(0,0,0,0.75)),url(background.jpg);
    background-size: cover;
    background-position: center;
    
}
.navbar{
    width: :85%;
    margin: auto;
    padding: 35px 0;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.logo{
    width: 120px;
    cursor: pointer;
}
.navbar ul li{
    list-style: none;
    display: inline-block;
    margin: 0 20px;
    position: relative;
}
.navbar ul li a{
    text-decoration: none;
    color: #fff;
    text-transform: uppercase;

}
.navbar ul li::after{
    content: '';
    height: 3px;
    width: 100%;
    background: #009688;
    position: absolute;
    left: 0;
    bottom: -10px;
    transition: 0.5s;
    
}
.navbar ul li:hover::after{
    width: 100%;
}
.content{
    width: 100%;
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    text-align: center;
    color: #fff;
    
}
.content h1{
    font-size: 70px;
    margin-top: 80px;
}
.content p{
    margin: 20px auto;
    font-weight: 100;
    line-height: 25px;
}
button{
    width: 200px;
    padding: 15px;
    text-align: center;
    margin: 20px;
    border-radius: 25px;
    font-weight: bold;
    border: 2px solid #009688;
    background: transparent;
    color: #fff;
    cursor: pointer;
    position: relative;
    overflow: hidden;
    
    
}
span{
    background: #009688;
    height: 100%;
    width: 0;
    border-radius: 25px;
    position: absolute;
    left: 0;
    border: 0;
    z-index: -1;
    transition: 0.5s;
}
button:hover span{
    width: 100%;
}
button:hover{
    border: none;
}



                
    
    
</body>
</html>
