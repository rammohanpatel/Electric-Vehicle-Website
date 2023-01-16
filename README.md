# Electric-Vehicle-Website
This website allows user to check for availability of electric vehicle in showroom and book a test ride.


//HTML
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Electric Scooties</title>
    <link rel="stylesheet" href="project1.css">
</head>


<body>
    
    <div class="banner">
        <div class="navbar">
          <img src="img/logo2.png" class="logo">
             <ul>
                <li><a href="#">Home </a></li>
                <li><a href="#">About Us </a></li>
                <li><a href="#">Contact Us </a></li>
             </ul>
        </div> 
    </div>
    <div class="content">
        <h1>Best Electric Scooters Are Here</h1>
        <p>Equipped with best and latest technology</p>
        <div>
            <button type="button"><span></span>BUY NOW</button>
            <button type="button"><span></span>TAKE A TEST DRIVE</button>
        </div>
    </div>
    
</body>
</html>


//CSS

.content,
button {
    text-align: center
}

.logo,
button {
    cursor: pointer
}

.navbar ul li::after,
span {
    width: 0;
    position: absolute;
    left: 0;
    transition: .5s
}

* {
    margin: 0;
    padding: 0;
    font-family: sans-serif
}

.banner {
    width: 100%;
    height: 100vh;
    background-image: url('img/Scooty3.jpg');
    background-size: cover;
    background-position: center
}

.navbar {
    width: 85%;
    margin: auto;
    padding: 35px 0;
    display: flex;
    align-items: center;
    justify-content: space-between
}

.logo {
    width: 120px
}

.content,
.navbar ul li:hover::after {
    width: 100%
}

.navbar ul li {
    list-style: none;
    display: inline-block;
    margin: 0 20px;
    position: relative
}

.navbar ul li a {
    text-decoration: none;
    color: #fff;
    text-transform: uppercase
}

.navbar ul li::after {
    content: '';
    height: 3px;
    background: #bef01a;
    bottom: -10px
}

.content {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    color: #f1cf0e
}

button {
    width: 200px;
    padding: 15px 0;
    margin: 20px 10px;
    border-radius: 25px;
    font-weight: 700;
    border: 2px solid #340096;
    background: transpaent;
    color: #171414;
    position: relative;
    overflow: hidden
}

span {
    background: #1529ab;
    height: 100%;
    border-radius: 25px;
    bottom: 0;
    z-index: -100
}

button:hover span {
    width: 100px;
    border: none
}
