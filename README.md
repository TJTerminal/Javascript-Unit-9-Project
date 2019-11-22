<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<title>Ted's site</title>
	<link rel="stylesheet" type="text/css" href="css/style.css">
</head>
<body>
	<header>
		<nav class='menu'>
			<div class='title'>
				<h1>Monk's Cafe</h1>
				<h3>"The Coffee Shop"</h3>
			</div>
			<br>
			<div class='navbar'>
				<h3><a href='#'>Reservations</a></h3>
					<h3><a href='#'>Make a Reservations</a></h3>
					<form>
						<input type="name" placeholder="">
						<button>Confirm Reservation</button>
					</form>
					<h3><a href='#'>Existing Reservations</a></h3>
					<table style='width:25%'>
						<tr>
							<th>Name</th>
							<th>Day</th>
						</tr>
						<tbody></tbody>
					</table>
				<br>
				<h3><a href='#'>Come Dine with Us</a></h3>
				<br>
				<h3><a href='#'>Customer Reviews</a></h3>
					<h4>"Big lettuce, big carrots, tomatoes like volleyballs."</h4>
					<h4>-Jerry Seinfeld, on The BIG Salad</h4>
				
			</div>
		</nav>




	<script type="text/javascript" src="js/script.js"></script>
</body>
</html>


CSS

.menu{
	border: none;
}

.navbar{

}

ul li {
	list-style: none;
}


Javascript

function map() {
	navigator.geolocation.getCurrentPosition(function(position) {
    var userLocation = {
      lat:  40.8054491,
      lng: -73.9654415
    };

    var map = new google.maps.Map(document.getElementById('map'), {
        center: userLocation,
        zoom: 10,
        scrollwheel: false
      });
    
    var marker = new google.maps.Marker ({
      position: userLocation,
      map: map,
      title: 'User Location'
    });
    
  });
}
