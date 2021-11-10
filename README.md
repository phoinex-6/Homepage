# Homepage
{% load static %}
<!DOCTYPE html>

<html lang="en">
	
	Carlo 
	<!--HEADER-->
	<head>
	  <title>Automate Food Service</title>
	  <meta charset="utf-8">
	  <meta name="viewport" content="width=device-width, initial-scale=1">
        

      <!--FOR FONT-->
      <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Trirong">

      <!--Bootstrap for the buttons-->
	 <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/css/bootstrap.min.css">
	  <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
	  <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.4.1/js/bootstrap.min.js"></script>
	  
	  <!--Style sheet Layout-->
	  <link rel="stylesheet" href="{% static 'styles.css' %}">
	</head>
	
	<body>
        <p style="text-align:center;">
            <img src="{% static 'project/img/junimo5.png' %}" style="width:200px; height:200px;">
        </p>
        <!--Homebuttons-->
		<div class="container">
           <br>
                <div class="container2" >
                    <p style="font-size: large; font-family: Trirong;" >
                        <div class="row justify-content-center align-items-center h-10" style="padding-left: 70px;padding-top: 10px;">
                        <div class="col-lg-11 col-sm-11 col-md-4 well well-lg" style="background-color: #ECE3A1; border-color: black; border-width: 5px;">
                        <legend style="border-width: 5px; border-color: black;"><a href=""><i class=""></i></a> Sign in!</legend>
                        
                        <form action="/homepage/" method="post" class="form" role="form">
                            {% csrf_token %}
                        <input class="form-control" name="youremail" placeholder="Username" type="email"required autofocus />
                        <input class="form-control" name="password" placeholder="Password" type="password" reuired/>
                        <br>
                         
                        <button class="btn btn-lg btn-primary btn-block" type="submit">
                                Sign in
                        </button>        
                        </form>
                        <a href="../signup">
                            <button class="btn btn-lg" type="submit">
                                Sign Up
                             </button>
                        </a>
                    </div>
                    </div>
                    </p>
                </div><br>
        </div>
		<!--FOOTER-->
		<footer>
			<p style="text-align:center; color:white;">RIEL JASPER ABANGAN, HANNAH MHAE LAQUINON CSIT327 G2-C1 AY 2021 - 2022</p>
		</footer>
		
	
	
	</body>


</html>
