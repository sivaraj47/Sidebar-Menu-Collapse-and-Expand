# Sidebar-Menu-Collapse-and-Expand-Html-Css-Javascript Responsive Sidebar Menu collapse and Expand | Professional Sidebar Menu collapse and Expand | Responsive Sidebar Menu and Dashboard
The  sidebar menu collapse and expand design is developed by html, css, javascript coding used to develop it and fully responsive design with flex concept used in the card design model for develop or create the template, website or design quickly and more user friendly for the developer or designer to easy customize the designs.


A sidebar menu is a great way to provide navigation options on a website. This project demonstrates how to create a responsive sidebar menu that can be collapsed and expanded using HTML, CSS, and JavaScript. This feature is especially useful for saving screen space and enhancing user experience.


This sidebar menu can be customized further to fit different designs and requirements. The provided code is a basic implementation and can be extended with additional features such as animations or responsive adjustments.

Feel free to modify and enhance the code to better suit your project needs.


<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">  
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no">
    	<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
    <title> Sidebar Menu collapse and Expand | Responsive Sidebar Menu collapse and Expand | Professional Sidebar Menu collapse and Expand | Responsive Sidebar Menu and Dashboard</title>    
    <meta name="description" content="The  sidebar menu collapse and expand design is developed by html, css, javascript coding used to develop it and fully responsive design with flex concept used in the card design model for develop or create the template, website or design quickly and more user friendly for the developer or designer to easy customize the designs." />
	
	<meta name="keywords" content="codingwithssr, sidebar menu collapse and expand html css w3schools, sidebar menu collapse and expand html css github, sidebar menu collapse and expand html css without,
sidebar menu collapse and expand html css example,
expand collapse sidebar menu,
bootstrap sidebar menu collapse with icon,
collapsible sidebar codepen,
collapse sidebar Bootstrap, expand collapse sidebar menu html css javascript
" />
	
	<meta name="author" content="https://codepen.io/codingwithssr" />
    <!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-KL9C7XQPJP"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-KL9C7XQPJP');
</script>
<!-- Google tag (gtag.js) this script for promote the code in google analytics-->
    <!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-M3N8GX9J');</script>
<!-- End Google Tag Manager -->
  </head>

<div class="wrapper">  
<nav id="sidebar">  
  <div class="head">    
    <h2 class="fulhide">      
      Codingiwithssr</h2>
    <h4 class="active">CSSR</h4>
  </div>
 <ul>    
   <li><a href=""><i class="fa fa-home" style="font-size:24px"></i> <span>Home</span><p>Home</p></a>   
   </li><li><a href=""><i class="fa fa-user" style="font-size:24px"></i> <span>About</span><p>About</p></a></li>
   <li><a href=""><i class="fa fa-sitemap" style="font-size:24px"></i> <span> Service</span><p> Service</p></a></li>
   <li><a href=""><i class="fa fa-puzzle-piece" style="font-size:24px"></i> <span>Project</span> <p>Project</p></a></li>
   <li><a href=""><i class="fa fa-map-marker" style="font-size:24px"></i> <span>Contact</span><p>Contact</p></a>
   </li>
 </ul>
</nav>
<div id="content">
  <div class="menu" onclick="toggleBtn()">
    <div class="bar1"></div>
      <div class="bar2"></div>
     <div class="bar3"></div>
  </div>
  <h2>Welcome to Dashboard !</h2>
</div>
</div>



@import url('https://fonts.googleapis.com/css?family=Poppins:400,500,600,700&display=swap');

*{
  margin:0;
  padding:0;
  user-select:none;
  box-sizing:border-box;
   font-family: 'Poppins', sans-serif;
  font-weight:500;
}
.head{
  padding:30px;
}
#sidebar { 
   width: 250px;
    position: fixed;
    top: 0;
    left: 0;
    height: 100vh;   
    background: #035992;
    color: #fff;
    transition: all 0.3s ease;
}

#sidebar.active{
  width:90px;  
  transition: all 0.3s ease;   
}
#sidebar.active:hover{
  overflow:auto;
  scrollbar-width:thin; 
}
#sidebar.active h4.active{  
  display:block;
}
#sidebar h4.active{  
  display:none;
  transition: .4s;
}
#sidebar.active h2.fulhide{ 
  display:none;
}
#sidebar.active ul li a{
 font-size:14px; 
  padding:10px;
  text-align:center;
  transition: all 0.3s ease;
}
#sidebar ul li a p{
  display:none;
}

#sidebar.active ul li a span, i{
  display:none;
  color:#fff;
}
/*#sidebar.active ul li:hover p{ 
  transition:all .3s ease;  
  display:block;*/
}
#sidebar ul{
  width:100%;
  height:100%;
  list-style:none;
  background:#ddf;
}
#sidebar ul li{
  line-height:60px;
  border-top:1px solid #9999;  
}
#sidebar ul li a{
  padding-left:40px;
  display:block;
  width:100%;
  text-decoration:none; 
  color:#000;
  font-weight:600;
  font-size:19px;
  transition: all 0.3s ease;
}
#sidebar ul li a span{
  color:#fff;
}
.menu{
  position:absolute;
  left:20px;
  top:10px;
}
 .bar1, .bar2, .bar3{
  width:29px;
  height:3px;  
  background:#000;
  margin:4px;
}
.wrapper{
  display:flex;
  width:100%;
}
#content.active {
    width: calc(100% - 90px);   
}
#content {
	width: calc(100% - 250px);
    padding: 20px;
    min-height: 100vh;
    transition: all .3s ease;
    position: absolute;
    top: 0;
    right: 0;   
   transition: all .3s ease;
  display:flex;
  justify-content:center;
  align-items:center;
}


function toggleBtn() {  document.getElementById('sidebar').classList.toggle('active');
  document.getElementById('content').classList.toggle('active');                    
}
