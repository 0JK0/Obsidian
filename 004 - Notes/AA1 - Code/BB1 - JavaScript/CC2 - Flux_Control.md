#JavaScript #Code  

# ^ If

-> You know if bro

	if (a < 2) {
		console.log("nel bro");
	
	} else {
		console.log("yes bro");
	}

-> There is also **Else if** but we both know what it does


# ^ While

-> a while loop, what did you expect???

	let i = 0;

	while ( i < 10){
		console.log(i);
		i++;
	}

-> Avoid Infinite loops, this are when the "(  )" are never fulfilled

-> **Do While** Slightly different from "While", the difference is, it first executes the code then loops

# ^ For

-> a for loop Duh

	for (incializacion, Comparacion, Terminacion) { code; }

-> Just a quick little snippet for checking if a number is even or odd?

	for( i = 0; i < 20, i++) {
	
		if (i % 2 == 0){
			console.log(i, " es impar")	
		}
	}

# ^ for of

-> Loop an array or list

	let animals = ["Pig","Cow","Dog"];

	for (let animal of animals){
		console.log(animal);
		
	}

# ^ For in

-> Loop for the property inside the array list instead of the ID

	let user = {
		id:1,
		name: "Pig",
		age: 2,
	}

	for (let prop in user){
		console.log(user[prop];) // prop.user[prop]
	}

# ^ Break and Continue

-> Skips a loop when certain conditions are meet, or continues the loop jumping one iteration of it

	let i = 0;

	while(i < 6){
	
		i++;
		if (i == 2 ) { continue; } // jumps one loop and continues

		if (i == 4) { break; } // Stops the code

		console.log(i);

	}


# ^ Switch

-> similar to **IF** but ir depends in if a variable is **TRUE**, basically alot of **IFs** stored in one,recommended instead of several **IF Else** 

	Let accion = "x";

	switch (accion) {

		case "A" :
			console.log("A");
			break;

		case "B" :
			console.log("B");
			break;

		case "C" :
			console.log("C");
			break;

		Default :
			console.log("Nahh");
	}

