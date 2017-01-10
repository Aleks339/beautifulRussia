<script type="text/javascript">
	
	var user_name;
	user_name = prompt("What is your name?");
	alert("Welcome to my page, " + user_name + "!");
	document.getElementById("welcome").innerHTML = 
	("Welcome to my page, " + user_name + "!");
	
	var d = new Date();
	document.getElementById("date").innerHTML = d.toDateString();
		
	var now = new Date();
var hrs = now.getHours();
var msg = "";

if (hrs >  0) msg = "Mornin' Sunshine!"; // REALLY early
if (hrs >  6) msg = "Good morning!";      // After 6am
if (hrs > 12) msg = "Good afternoon!";    // After 12pm
if (hrs > 17) msg = "Good evening!";      // After 5pm
if (hrs > 22) msg = "Go to bed!";        // After 10pm

document.getElementById("goodTime").innerHTML = msg;
	
	var getUp = new Date();
	if (hrs < 12) msg = "Get up! Quickly!";
	else{
		msg = ""
	}
	document.getElementById("getUp").innerHTML = msg;
	
var randomFact = 
["77% of Russia is made up of Siberia.", 
"A russian woman in the 1700s gave birth to 16 pairs of twins, 7 sets of triplets and 4 sets of quadruplets in just 40 years with the same man.", 
"In 1908 the Imperial Russian Olympic Team arrived in London 12 days too late for the games because they were not using the Gregorian calendar yet.", 
"The oldest plant ever to be regenerated has been grown in Russia from 32,000-year-old seeds.",
"There was a 'Beard Tax' in Russia, during Peter the Great's Reign, paid by anyone who had a beard.", 
 "There's a museum in Russia that hires cats to protect its artworks against rodents.",
 "20% of the world's unfrozen fresh water is in a single lake: Russia's Lake Baikal.",
 "In Canada, Mexico, India, Russia and Israel, bank notes have Braille-like markings on them for the blind."
];
	


var randFact = randomFact[Math.floor(Math.random() * randomFact.length)];

document.getElementById("randomFact").innerHTML = randFact;
	
	</script>