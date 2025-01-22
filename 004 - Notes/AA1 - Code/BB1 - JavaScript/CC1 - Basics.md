#Theme-Basics #JavaScript #Code  

01/15/2024/Wed

# ^ Set Up

	 < Script > < Script />

	< Script src="./app.js" > < Script />

# ^ Language Basics

-> **Let** used to define variables, after defining its not needed 

	Let nombre = "A";

-> **Console.log** Used for console printing

	console.log(nombre);

-> **Const** Doesn't allow to modify the variable later on

	const A = "name";

->  **Typeof** Brings the type of the variable

	console.log(typeof nombre); = string

# ^ Objetos

-> **{  }** i fee like they are similar to dictionaries, By default these are unorganized is recommended   to always leave a comma at the end so it causes no issues if you later add on trough a function or loop

	let personaje = {
		nombre : "tanjiro",
		anime: "Demon Slayer"
		edad: 16,
	}

Since this are unorganized, when you want to point to a specific property

	console.log(personaje.nombre); // tanjiro
	console.log(personaje[anime]); // Demons Slayer

If you want to modify a property or  **delete** a property

	personaje.edad = 16;
	delete personaje.anime;

## ^ Array

-> **[  ]** basically a list AKA array, this are indeed organized

	let animal = ["cat","dog"];

not much else to say only interesting bit is that you can leave empty spots by assigning to a further one;

	let you = ["a","b","c"];
	  
	you[8] = "z"; 

	// you = ["a","b","c", , , , ,"z"]
 

## ^ Functions

-> Well functions no much science to it

	function saludar(){ console.log("A"); }

	saludar();

-> **Return** for when the function need to return a value or another function even

	funtion suma(){
		return 2 + 2;
	}

-> **Arguments** Do i really have to explain how to pass info?

	function suma(a,b) {
		return console.log(a + b); 
	}


# !
-> Wont be taking notes of unnecessary stuff, so stuff that doesn't change between languages like why write down the "ABC" when learning another romance language 

-> Mentioned stuff like arithmetic symbols, comparison symbols, incrementes and boolean checks, greater than lesser than "> , <", comparison tables

-> The "&&" , "or", "not" logical operators, again same in every language 

**! 1:44:40 --> skip --> 2:00:41** stuff which i found none important at the current moment [[CC3 - Extra]]



