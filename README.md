<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0"> <!-- displays site properly based on user's device -->

  <link rel="icon" type="image/png" sizes="32x32" href="./images/favicon-32x32.png">
  
  <title>Frontend Mentor | Intro section with dropdown navigation</title>
  <link  rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
  </header>
  <nav>
    <ul class="sidebar">
       <li onclick="hideSidebar()"><a href="#"><svg width="26" height="26" xmlns="http://www.w3.org/2000/svg"><g fill="#151515" fill-rule="evenodd"><path d="m2.393.98 22.628 22.628-1.414 1.414L.979 2.395z"/><path d="M.98 23.607 23.609.979l1.414 1.414L2.395 25.021z"/></g></svg></a></li> 
      <li><a href="#">Features</a>
      </li> 
      <li><a href="#">Companies</a>
      <li><a href="#" class="hideOnMobile">Contact</a></li>
      <li><a href="#" class="hideOnMobile">About</a></li>
      <li><a href="#" class="hideOnMobile">Login</a></li>
      <li><a href="#" class="hideOnMobile">Register</a></li>
    </ul>
    <ul>
       <li class="logo"><a href="#">Snap</a></li>
      <li><a href="#">Features</a>
      </li>
      <li><a href="#">Companies</a>
      </li>
      <li><a href="#">Contact</a></li>
      <li><a href="#">About</a></li>
      <li><a href="#" id="menu">Login</a></li>
      <li><a href="#" id="menu2">Register</a></li>
      <li  class="menu-button" onclick="showSidebar()"><a href="#"><img src="images/icon-menu.svg"></a></li>
    </ul>
  </nav>
  <section style="margin:5rem;">
    <div  style=" height:100%;width:100%">
      <img src="images/image-hero-desktop.png"  class ="hero-img" style="
       float:right; margin-right: 4rem; margin-bottom:4rem; display: flex;
       height:50%;width:50%
      ">
    <div class="hero" style="font-size:2rem">
      <h2 style="color:black;font-size:4rem; margin-bottom:2rem; font-weight:10rem;">Make <br> remote work</h2><br><br>
      <p  class="intro"></p>
        Get your team in sync, no matter your location.<br>
        Streamline processes, create team rituals, and
      <br> watch productivity soar.
      </p>
    </div>
      <button href="#" class="click">Learn more</button>
      <style>
        .click{
          background-color:white;
          border:none;
          margin-top:4rem;
          font-size:1.2rem;
          padding:25px;
          color:grey
        }
        .click:hover{
          background-color:black;
          color:white;
          border-radius:15px;
          padding:25px;
        }
        p{
          color:grey;
        }
        .icons{
          margin-top:20%;
          margin-bottom:15%
        }
        @media(max-width:800px ){
        .hero-img{
          display:flex;
        }
      }
        @media(max-width:480px ){
        .hero-img{
          display:flex;
        }
        }
      </style>
    </div><br>
  </div class="icons"><br>
  <img src="images/client-databiz.svg" alt="">&nbsp;&nbsp;
  <img src="images/client-audiophile.svg" alt="">&nbsp;&nbsp;
  <img src="images/client-meet.svg" alt="">&nbsp;&nbsp;
  <img src="images/client-maker.svg" alt="">&nbsp;&nbsp;
  <div>
  </section>
  <div class="attribution">
    Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
    Coded by <a href="#">Divine Obute Ene</a>.
  </div>
  <script src="index.js"></script>
  <!-- <script>
    function showSidebar(){
  const sidebar = document.querySelector('.sidebar')
  sidebar.style.display = "flex";
};

function hideSidebar(){
  const sidebar = document.querySelector('.sidebar')
  sidebar.style.display = "none";
} -->
  </script>
</body>
</html>
*{
  margin:0;
  padding:0;
}
body{
  min-height:100vh;
  background-color: rgb(250, 250, 250);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

  nav{
background-color: whitesmoke;
box-shadow: 3px 3px 5px rgba( 105, 105, 105); 
} 
nav ul{
  width:100%;
  list-style:none;
 display: flex;
 justify-content: flex-end;
 align-items:center;
}
 nav li{
  height:50px;
}
nav a{
  height:100%;
  padding:0 30px;
  text-decoration:none;
  display: flex;
  align-items:center;
  color:grey
}
nav a:hover{
  color:black;
}
nav li :first-child{
  margin-right:60%;
}
 .menu :focus,
  .menu :active{
  background:black;
  color:white;
  border:2px;
 }
.sidebar{
  position:fixed;
  top:0;
  right:0;
  height:100vh;
  width:250px;
  z-index:999;
  background-color: rgba(255, 255, 255, 0.2);
  backdrop-filter:blur(10px);
  display:flex;
  flex-direction: column;
  align-items:flex-start;
  justify-content:flex-start;
}
.sidebar li{
  width:100%;
}
.sidebar a{
  width:100%;
}
.menu-button{
  display:none
}

@media(max-width: 800px){
  .hideOnMobile{
    display:none;
  }
  .menu-button{
    display:block;
  }
  .hero-img{
    display:flex;
  }
}
@media (max-width:480px) {
  .hideOnMobile{
    display:none;
  }
  .menu-button{
    display:block;
  }
  .hero-img{
    display:flex;
  }
}

 .logo{
  margin-right:60%;
  font-weight:200px;
} 

.section{
  margin:5rem;
}


