<html>
<head>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
<link rel="shortcut icon" href="favicon.ico">
<script src="http://code.jquery.com/jquery-3.5.1.js"></script>
<script>
  $(document).ready(function(){
    $('#icon').click(function(){
	  $('ul').toggleClass('show');
	});
  });
</script>
<script>
$(window).scroll(function(){
	if ($(window).width() >= 909){	
		window.onscroll = function() {scrollFunction()};

  function scrollFunction(x) {
    if (document.body.scrollTop > 80 || document.documentElement.scrollTop > 80) {
        document.getElementById("nav").style.height = "80px";
		document.getElementById("nav").style.backgroundColor = "#3e3e3e";
		document.getElementById("logo").style.fontSize = "45px";
		document.getElementById("logo").style.paddingTop = "10px";
		document.getElementById("logo").style.textStroke = "2px black";
		document.getElementById("list").style.paddingTop = "30px";
   } 
  else {
    document.getElementById("nav").style.height = "120px";
   document.getElementById("nav").style.backgroundColor = "transparent";
    document.getElementById("logo").style.fontSize = "55px";
    document.getElementById("logo").style.paddingTop = "20px";
	document.getElementById("logo").style.textStroke = "2px black";
	document.getElementById("list").style.paddingTop = "50px";
  }
}
}
});

</script>

<style>
*{
  margin:0;
  padding:0;
  box-sizing: border-box;
  text-decoration: none;
  list-style: none;
}

body{
  font-family: arial;
}
nav{
  position: fixed; 
  width: 100%;
  height: 120px;
  background-color: transparent;
  z-index: 1000;
  transition: all .5s;
}
div.logo{
  float: left;
  font-size:  65px;
  font-weight: bold;
  color: transparent;
  -webkit-text-stroke: 2px white;
  letter-spacing: px;
  padding: 20px 100px;
  transition: all .5s;
}

nav ul{
  float: right;
  margin-right: 40px;
  padding: 70px 0px;
  transition: all .5s;
  z-index: 1000;
}
nav ul li{
  display: inline-block;
  margin: 0 5px;
  transition: all .5s;
  cursor: pointer;
}
nav ul li a{
  padding: 7px 10px;
  color: white;
  font-size: 18px;
  text-transform: uppercase;
  border: 1px solid transparent;
  border-radius: 4px;
  transition: all .5s;
}
a:hover {
  background-color: white;
  color: black;  
}
a.active{
  border: 2px solid white;
  border-radius: 4px;
}
nav #icon{
  color: white;
  font-size: 30px;
  line-height: 100px;
  float: right;
  margin-right: 40px;
  cursor: pointer;
  padding-top: 34px;  
  display: none;
}
.firstbg{
  position: relative;
  width: 100%;
  background-image: repeating-linear-gradient(135deg, #ed2c1d , #ef5044 150px);
  border: 2px solid black;

}
.firstbgcon{
  margin: 25%;
  margin-top: 20%;
  border-top: 1px solid #37e5fa;
  border-bottom: 1px solid #37e5fa;
  padding: 20px;

}
.firstbgcon h3{
  font-size: 25px;
  text-align: center;
  user-select: none;
  
}
.vismisrow{
  width: 100%;
  height: 50%;
  margin-top: 100px;
}
.mission , .vision{
  float: left;
  width: 45%;
  height: 85%;
  margin: 2%;
  padding: 1%;
  border-radius: 20px;
  background-image:  linear-gradient(135deg, #0d0c0a 0%, #32312f 100%);
  border: 5px solid black;
  box-shadow: 15px 15px 15px grey;
  user-select: none;
}
.mission h3 , .vision h3{
  font-size: 250%;
  color: #8e8e8d;
  text-align: center;
}
u{
  text-decoration-line: underline;
  text-decoration-style: solid;
  text-decoration-color: #aec9e8;
}
.miscon , .viscon{
  text-align: center;
  margin: 1%;
  width: 100%;
  color: white;
  padding: 2% 10% ;
  font-size: 150%;
  background-color: ;
  margin: relative;
}
.viscon{
  font-size: 160%;
  padding: 8% 10%;
}
.proandser{
  width: 100%;
}
.service-section{
  background-color: grey;
  background-size: cover;
  padding: 60px 0;
  margin-top: 100px;
}
.innerwidth{
  width: 100%;
  max-width: 1200px;
  margin: auto;
  padding: 0 20px;
  overflow: hidden;
}
.section-title{
  text-align: center;
  color: #ddd;
  text-transform: uppercase;
  font-size: 30px;
}
.border{
  width: 160px;
  height: 2px;
  background: #82ccdd;
  margin: 40px auto;
}
.service-container{
  display: flex;
  flex-wrap: wrap;
  justify-content: center; 
  user-select: none;
}
.service-box{
  max-width: 24.33%;
  padding: 10px;
  text-align: center;
  color: #ddd;
  cursor: pointer;
}
.service-icon{
 display: inline-block;
 width: 70px;
 height: 70px;
 border: 3px solid #82ccdd;
 color: #82ccdd;
 transform: rotate(45deg);
 margin-bottom: 30px;
 margin-top: 16px;
 transition: 0.3s linear;
}
.service-icon i{
  line-height: 70px;
  transform: rotate(-45deg);
  font-size: 26px;
}
.service-box:hover .service-icon{
  background: #82ccdd;
  color: #ddd;
}
.service-title{
  font-size: 18px;
  text-transform: uppercase;
  margin-bottom: 10px;
}
.service-desc{
  font-size: 14px;
}
.project{
  width: 100%;
  padding-top: 5px;
  margin-top: 0;
  background-image: linear-gradient(45deg , #ffcc5c 20%, #8ad267 20% 50%, #ff6f69 50% 80%, #96ceb4 80%);
}
.projecthead{
   margin-top: 8%;
   padding-left: 15%;
   transform: uppercase;
   text-align: left;
   font-size: 190%;
}
.borderbox{
  width: 30%;
  height: 2px;
  margin-left: 10%;
  margin-top: 20px;
  border-top: 2px solid blue;
}
.pro{
  width:80%;
  margin: 5% 5% 0% 7%;
  padding: 1% 1% 1% 3%; 
  border-bottom: 2px solid black;

}
.pro h4{
   font-size: 280%;   
   width: 500px;	  
}
.pro.len h4{
  font-size: 250%;
  width: 550px;
}
.pro h6{
   padding: 3% 0% 3% 0%;
   font-size: 100%;
}
.morepost button{
  margin: 2% 10% 2% 65%;
  height: 6%;
  padding: 5px 5px 10px 15px;
  border-radius: 20px;
  background:#0099cc -webkit-linear-gradient(bottom,rgba(255,255,255,.2) 0%,rgba(0,0,0,.2) 100%);
}
.morepost h5{
  float: left;
  font-size: 18px; 
  padding-right: 6px;
  color: white;
}
.morepost i{
  padding: 7px 5px 5px 5px;
  color: white;
}
.morepost button:hover #proicon{
  background:#0099cc -webkit-linear-gradient(bottom,rgba(255,255,255,.2) 0%,rgba(0,0,0,.2) 100%);
}
@media (max-width: 1164px){
  div.logo{	
    font-size: 60px;
	padding-left: 50px;
	transition: all .5s;
  }
  nav ul{
	margin-right: 10px;
    transition: all .5s;
  }
  nav ul li{
    margin: 0 2px;
    transition: all .5s;
  }
  nav ul li a{
    font-size: 12px;
	font-weight: bold;
	padding: 7px 8px;
    transition: all .5s;
  }
  .miscon , .viscon{
  margin: 1%;
  padding: 1% 7% ;
  font-size: 100%;
  }
  .viscon{
    padding: 7% 7%;
  }
  .service-title{
    font-size: 14px;	
  }
  .service-desc{
    font-size: 11px;
  }
  .morepost button{
    margin: 2% 10% 2% 50%;
  }
}
@media (max-width: 909px){
  nav{
    height: 80px;
	width: 100%;
	background-color: #282626;
  }
  nav label#icon{
    float: right;
    display: block;	
	font-size: 25px;
	padding-top: 25px;
  }
  div.logo{   
    float: left;
    font-size: 35px;
	padding-left: 10px;
	color: white;
	-webkit-text-stroke: 0px white;
	transition: all .5s;
  }
  nav ul{
    position: fixed;
	width: 100%;
	height: relative;
	background: #3e3e3e;
	top: 80px;
	left: -100%;
	text-align: center;
	padding: 0px 0px 0px 0px;
	border-bottom-right-radius: 10px;
	border-bottom-left-radius: 10px;
	transition: all .5s;
  }
  nav ul li{
    display: block;
	margin: 20px 0 10px 0;
}
  nav ul li a{
    font-size: 15px; 
  }
  .firstbg{
    height: 100%;
  }
  .firstbgcon{
  padding: 5%;
  margin: 37% 10% 0 10%;
  
 }
 .firstbgcon h3{
   font-size: 16px;
 }
 .mission h3 , .vision h3{
   font-size: 180%;
 }
 .miscon , .viscon{
   font-size: 80%;
   padding: 1% 3%;
 }
 .viscon{
   font-size: 95%;
   padding: 15% 5%;
 }
  .service-box{
    max-width: 33.33%;
  }
   .service-title{
    font-size: 14px;	
  }
  .service-desc{
    display: none;
  }
  .projecthead{
    font-size: 150%;
  }
  .borderbox{
    width: 50%;
  }
  .pro{
    margin-left: 3%;
  }
  .pro h4{
    font-size: 120%;
	margin-left: 2%;
  }
  .pro h6{
    font-size: 90%;
  }
  .morepost button{
    margin: 4% 10% 4% 20%;
  }
  .morepost h5{
    font-size: 100%;
	padding: 3px 2px 0 0;
  }
  .morepost i{
    padding-bottom: 5px;
	font-size: 80%;
  }
  nav ul.show{
    left: 0;
  }
}
</style>
</head>
<body>
 <nav id="nav">
    <div class="logoimg"></div>
    <div class="logo" id="logo">Epoch Zero</div>
	<label id="icon">
	   <i class="fa fa-bars" ></i>
	</label>
    <ul id="list">
      <li class="liactive"><a class="active" href="#">Home</a></li>	
      <li ><a href="#">key project</a></li>	
      <li><a href="#">client testimonial</a></li>	
      <li><a href="#">carrer</a></li>	
      <li><a href="#">contact</a></li>	
	</ul>
  </nav>
  <div class="firstbg">
    <div class="firstbgcon"><h3>
	Lorem Ipsum is simply dummy text of the printing and typesetting industry.
	Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
	when an unknown printer took a galley of type and scrambled it to make a type specimen book.
	</h3></div>
  </div>
  <div class="vismisrow">
    <div class="mission">
	  <div class="mishead"><h3><u>Mission</u></h3><br></div>
	  <div class="miscon">
	    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
	    Lorem Ipsum has been the industry's standard dummy text ever since the 1500s.
      </div>
	</div>
    <div class="vision">
      <div class="vishead"><h3><u>Vision</u></h3></div>
	  <div class="viscon">
	    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
	  </div>
	</div>
  </div>
  <div class="service-section">
   <div class="innerwidth">
     <h1 class="section-title">Prodoct and Services<h1>
	 <div class="border"></div>
	 <div class="service-container">
	  <div class="service-box">
	   <div class="service-icon">
	     <i class="fa fa-cloud"></i>
	   </div>
		 <div class="service-title">Cloud Service</div>
		 <div class="service-desc">
		   Lorem Ipsum is simply dummy text of the printing and typesetting industry.
		   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s
		 </div>
	 </div>
	 	  <div class="service-box">
	   <div class="service-icon">
	     <i class="fa fa-paint-brush"></i>
	   </div>
		 <div class="service-title">UI/UX Design</div>
		 <div class="service-desc">
		   Lorem Ipsum is simply dummy text of the printing and typesetting industry.
		   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
		   when an unknown printer took a galley of type and scrambled it to make a type specimen book.

		 </div>
	 </div>
	 	  <div class="service-box">
	   <div class="service-icon">
	     <i class="fa fa-code"></i>
	   </div>
		 <div class="service-title">Web Development</div>
		 <div class="service-desc">
		   Lorem Ipsum is simply dummy text of the printing and typesetting industry.
		   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s
		 </div>
	 </div>
	 	  <div class="service-box">
	   <div class="service-icon">
	     <i class="fa fa-mobile-phone"></i>
	   </div>
		 <div class="service-title">Application Development</div>
		 <div class="service-desc">
		    Lorem Ipsum is simply dummy text of the printing and typesetting industry.
		   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
		   when an unknown printer took a galley of type and scrambled it to make a type specimen book.
		 </div>
	 </div>
	 	  <div class="service-box">
	   <div class="service-icon">
	     <i class="fa fa-gears"></i>
	   </div>
		 <div class="service-title">Maintenance and Support Services</div>
		 <div class="service-desc">
		   Lorem Ipsum is simply dummy text of the printing and typesetting industry.
		   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s
		 </div>
	 </div>
	 	  <div class="service-box">
	   <div class="service-icon">
	     <i class="fa fa-television"></i>
	   </div>
		 <div class="service-title">Software Development</div>
		 <div class="service-desc">
		   Lorem Ipsum is simply dummy text of the printing and typesetting industry.
		   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
		   when an unknown printer took a galley of type and scrambled it to make a type specimen book.
		 </div>
	 </div>
	 	  <div class="service-box">
	   <div class="service-icon">
	     <i class="fa fa-bullhorn"></i>
	   </div>
		 <div class="service-title">Digital Marketing</div>
		 <div class="service-desc">
		   Lorem Ipsum is simply dummy text of the printing and typesetting industry.
		   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s
		 </div>
	 </div>
	 	  <div class="service-box">
	   <div class="service-icon">
	     <i class="fa fa-credit-card"></i>
	   </div>
		 <div class="service-title">E-commerce Development</div>
		 <div class="service-desc">
		   Lorem Ipsum is simply dummy text of the printing and typesetting industry.
		   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
		   when an unknown printer took a galley of type and scrambled it to make a type specimen book.	
		 </div>
	 </div>
	</div>
   </div>
  </div>
  <div class="project">
    <div class="projecthead">
	  <h2>PROJECT</h2>
	</div>
	<div class="borderbox"></div>
	<div class="pro">
	  <h4>ProjectOne</h4>
	  <h6>
	   Lorem Ipsum is simply dummy text of the printing and typesetting industry
	  </h6>
	</div>  
	<div class="pro">
	  <h4>ProjectTwo</h4>
	  <h6>
	   Lorem Ipsum is simply dummy text of the printing and typesetting industry.
	   Lorem Ipsum has been the industry's standard dummy text ever since the 1500s,
	   when an unknown printer took a galley of type and scrambled it to make a type specimen book.
	  </h6>
	</div>
    <div class="morepost">
	  <button><a href=""><h5>Check out our Latest Work</h5><i class="fa fa-chevron-right" id="proicon"></i></a></button>
	</div>
  </div>
</body>
</html>
</html>
