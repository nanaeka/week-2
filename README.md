# Writing week-2

# Javascript – Scope
  Scope adalah konsep dalam flow data variabel.Menentukan suatu variabel bisa diakses pada scope tertentu atau tidak.

- Blocks
  
  Blocks adalah code yang berada didalam curly braces {}.Conditional, function, dan  looping menggunakan blocks.

- Global Scope
   
   berarti variabel yang kita buat dapat diakses dimanapun dalam suatu file.Agar menjadi Global Scope, suatu variabel harus dideklarasikan diluar Blocks.

- Local Scope
   
   berarti kita mendeklarasikan variabel didalam blocks seperti function, conditional, dan looping.Maka variabel hanya bisa diakses didalam blocks saja. Tidak bisa diakses diluar blocks


# JAVASCRIPT – FUNCTION

  Function adalah sebuah blok kode dalam sebuah grup untuk menyelesaikan 1 task/1 fitur. Saat kita membutuhkan fitur tersebut nantinya, kita bisa kembali menggunakannya.
  
  
 
 Parameter dan Argumen
 
 
•	Dengan parameter, function dapat menerima sebuah inputan data dan menggunakannya untuk melakukan task/tugas.

•	Saat membuat function/fitur, kita harus tahu data-data yang dibutuhkan. Misalnya saat membuat function penambahan 2 buah nilai. Data yang dibutuhkan adalah 2 buah nilai tersebut.

Argumen Function


•	Argumen adalah nilai yang digunakan saat memanggil function.

•	Jumlah argumen harus sama dengan jumlah parameternya

•	Jadi jika di function penambahan ada 2 parameter nilai saat membuat function. Saat memanggil function kita gunakan 2 buah nilai argumen.

  Nantinya saat kita mengembangkan aplikasi dengan skala besar, function sangat sangat dibutuhkan agar kita dapat dengan mudah memanage code dan tracing code jika ada error.


# Default Parameters

  Default paramaters digunakan untuk memberikan nilai awal/default pada parameter function.Default parameters bisa digunakan jika kita ingin menjaga function agar tidak error saat dipanggil tanpa argument.

# Function Helper
Kita bisa menggunakan function yang sudah dibuat pada function lain.

# Arrow Function
Arrow function adalah cara lain menuliskan function. Ini adalah fitur terbaru yang ada pada ES6 (Javascript Version)

# Short Syntax Function


# data types
  Programming languages all have built-in data structures, but these often differ from one language to another. This article attempts to list the built-in data structures available in JavaScript and what properties they have. These can be used to build other data structures. Wherever possible, comparisons with other languages are drawn.


# javascript types


The set of types in the JavaScript language consists of primitive values and objects.

•	Primitive values (immutable datum represented directly at the lowest level of the language)

•	Boolean type

•	Null type

•	Undefined type

•	Number type

•	BigInt type

•	String type

•	Symbol type

    
# Objects (collections of properties)


• Primitive values

All types except objects define immutable values (that is, values which can't be changed). For example, Strings are immutable. We refer to values of these types as "primitive values".


• Boolean type

Boolean represents a logical entity and can have two values: true and false. See Boolean and Boolean for more details.

• Null type

The Null type has exactly one value: null. See null and Null for more details.

• Undefined type

A variable that has not been assigned a value has the value undefined. See undefined and Undefined for more details.

• Numeric types

ECMAScript has two built-in numeric types: Number and BigInt — along with the related value NaN.

• Number type

  The Number type is a double-precision 64-bit binary format IEEE 754 value. It is capable of storing positive floating-point numbers between 2^-1074 (Number.MIN_VALUE) and 2^1024 (Number.MAX_VALUE) as well as negative floating-point numbers between -(2^-1074) and -(2^1024), but it can only safely store integers in the range -(2^53 − 1) (Number.MIN_SAFE_INTEGER) to 2^53 − 1 (Number.MAX_SAFE_INTEGER).




Values outside the range ±(2^-1074 to 2^1024) are automatically converted:


    • Positive values greater than Number.MAX_VALUE are converted to +Infinity.

    • Positive values smaller than Number.MIN_VALUE are converted to +0.

    • Negative values smaller than -Number.MAX_VALUE are converted to -Infinity.

    • Negative values greater than -Number.MIN_VALUE are converted to -0.


• BigInt type
 
 
  The BigInt type is a numeric primitive in JavaScript that can represent integers with arbitrary precision. With BigInts, you can safely store and operate on large integers even beyond the safe integer limit for Numbers.A BigInt is created by appending n to the end of an integer or by calling the constructor.


  You can obtain the largest safe value that can be incremented with Numbers by using the constant Number.MAX_SAFE_INTEGER. With the introduction of BigInts, you can operate with numbers beyond the Number.MAX_SAFE_INTEGER



•  NaN

NaN ("Not a Number") is typically encountered when the result of an arithmetic operation cannot be expressed as a number. It is also the only value in JavaScript that is not equal to itself.

•  String type

JavaScript's String type is used to represent textual data. It is a set of "elements" of 16-bit unsigned integer values. Each element in the String occupies a position in the String. The first element is at index 0, the next at index 1, and so on. The length of a String is the number of elements in it.


Use strings for textual data. When representing complex data, parse strings, and use the appropriate abstraction.

# Symbol type
A Symbol is a unique and immutable primitive value and may be used as the key of an Object property (see below). In some programming languages, Symbols are called "atoms".

For more details see the Symbol reference page.

•  Objects

In computer science, an object is a value in memory which is possibly referenced by an identifier.

•  Properties
In JavaScript, objects can be seen as a collection of properties. With the object literal syntax, a limited set of properties are initialized; then properties can be added and removed. Property values can be values of any type, including other objects, which enables building complex data structures. Properties are identified using key values. A key value is either a String value or a Symbol value.

There are two types of object properties: The data property and the accessor property. Each property has corresponding attributes. Each attribute is accessed internally by the JavaScript engine, but you can set them through Object.defineProperty(), or read them through Object.getOwnPropertyDescriptor(). You can read more about the various nuances on the Object.defineProperty() page.

# Data property
Data properties associate a key with a value. It can be described by the following attributes:

•  value
The value retrieved by a get access of the property. Can be any JavaScript value.

•  writable
A boolean value indicating if the property can be changed with an assignment.

•  enumerable
A boolean value indicating if the property can be enumerated by a for...in loop. See also Enumerability and ownership of properties for how enumerability interacts with other functions and syntaxes.

•  configurable
A boolean value indicating if the property can be deleted, can be changed to an accessor property, and can have its attributes changed.

# Accessor property
Associates a key with one of two accessor functions (get and set) to retrieve or store a value.

Note: It's important to recognize it's accessor property — not accessor method. We can give a JavaScript object class-like accessors by using a function as a value — but that doesn't make the object a class.

An accessor property has the following attributes:

•  get
A function called with an empty argument list to retrieve the property value whenever a get access to the value is performed. See also getters. May be undefined.

•  set
A function called with an argument that contains the assigned value. Executed whenever a specified property is attempted to be changed. See also setters. May be undefined.

•  enumerable
A boolean value indicating if the property can be enumerated by a for...in loop. See also Enumerability and ownership of properties for how enumerability interacts with other functions and syntaxes.

•  configurable
A boolean value indicating if the property can be deleted, can be changed to a data property, and can have its attributes changed.

# "Normal" objects, and functions
A JavaScript object is a mapping between keys and values. Keys are strings (or Symbols), and values can be anything. This makes objects a natural fit for hashmaps.

Functions are regular objects with the additional capability of being callable.

# Dates
When representing dates, the best choice is to use the built-in Date utility in JavaScript.

# Indexed collections: Arrays and typed Arrays
Arrays are regular objects for which there is a particular relationship between integer-keyed properties and the length property.

Additionally, arrays inherit from Array.prototype, which provides to them a handful of convenient methods to manipulate arrays. For example, indexOf() (searching a value in the array) or push() (adding an element to the array), and so on. This makes Arrays a perfect candidate to represent lists or sets.

Typed Arrays present an array-like view of an underlying binary data buffer, and offer many methods that have similar semantics to the array counterparts. "Typed array" is an umbrella term for a range of data structures, including Int8Array, Float32Array, etc. Check the typed array page for more information.

# Keyed collections: Maps, Sets, WeakMaps, WeakSets
These data structures take object references as keys. Set and WeakSet represent a set of objects, while Map and WeakMap associate a value to an object.



# String

  Strings are useful for holding data that can be represented in text form. Some of the most-used operations on strings are to check their length, to build and concatenate them using the + and += string operators, checking for the existence or location of substrings with the indexOf() method, or extracting substrings with the substring() method.
  
  
      const string1 = "A string primitive";
      const string2 = 'Also a string primitive';
      const string3 = `Yet another string primitive`;



Character access

There are two ways to access an individual character in a string. The first is the charAt() method:

      'cat'.charAt(1) // gives value "a"
      
      
Comparing strings

In C, the strcmp() function is used for comparing strings. In JavaScript, you just use the less-than and greater-than operators:

      const a = 'a';
      const b = 'b';
      if (a < b) { // true
        console.log(`${a} is less than ${b}`)
      } else if (a > b) {
        console.log(`${a} is greater than ${b}`)
      } else {
        console.log(`${a} and ${b} are equal.`)
      }


locale-aware manner.

String primitives and String objects

Note that JavaScript distinguishes between String objects and primitive string values. (The same is true of Boolean and Numbers.)

        const strPrim = "foo"; // A literal is a string primitive
        const strPrim2 = String(1); // Coerced into the string primitive "1"
        const strPrim3 = String(true); // Coerced into the string primitive "true"
        const strObj = new String(strPrim); // String with new returns a string wrapper object.

        console.log(typeof strPrim); // Logs "string"
        console.log(typeof strPrim2); // Logs "string"
        console.log(typeof strPrim3); // Logs "string"
        console.log(typeof strObj);  // Logs "object"




String coercion

Many built-in operations that expect strings first coerce their arguments to strings (which is largely why String objects behave similarly to string primitives). The operation can be summarized as follows:

• Strings are returned as-is.
• undefined turns into "undefined".
• null turns into "null".
• true turns into "true"; false turns into "false".
• Numbers are converted with the same algorithm as toString(10).
• BigInts are converted with the same algorithm as toString(10).
• Symbols throw a TypeError.
• Objects are first converted to a primitive by calling its [@@toPrimitive]() (with "string" as hint), toString(), and valueOf() methods, in that order. The resulting primitive is then converted to a string.


# Examples
String conversion

It's possible to use String as a more reliable toString() alternative, as it works when used on null and undefined. For example

		const nullVar = null;
		nullVar.toString();       // TypeError: nullVar is null
		String(nullVar);          // "null"

		const undefinedVar = undefined;
		undefinedVar.toString();  // TypeError: undefinedVar is undefined
		String(undefinedVar);     // "undefined"



# Number
Number is a primitive wrapper object used to represent and manipulate numbers like 37 or -9.25.

The Number constructor contains constants and methods for working with numbers. Values of other types can be converted to numbers using the Number() function.

Numbers are most commonly expressed in literal forms like 0b101, 0o13, 0x0A. The lexical grammar contains a more detailed reference.


		123; // one-hundred twenty-three
		123.0; // same
		123 === 123.0; // true

# Examples
Using the Number object to assign values to numeric variables
The following example uses the Number object's properties to assign values to several numeric variables:

		const biggestNum = Number.MAX_VALUE;
		const smallestNum = Number.MIN_VALUE;
		const infiniteNum = Number.POSITIVE_INFINITY;
		const negInfiniteNum = Number.NEGATIVE_INFINITY;
		const notANum = Number.NaN;

# Integer range for Number

		const biggestInt = Number.MAX_SAFE_INTEGER; //  (2**53 - 1) =>  9007199254740991
		const smallestInt = Number.MIN_SAFE_INTEGER; // -(2**53 - 1) => -9007199254740991


# Using Number() to convert a Date object

		const d = new Date("December 17, 1995 03:24:00");
		console.log(Number(d));

# Convert numeric strings and null to numbers
 
		Number("123"); // 123
		Number("123") === 123; // true
		Number("12.3"); // 12.3
		Number("12.00"); // 12
		Number("123e-1"); // 12.3
		Number(""); // 0
		Number(null); // 0
		Number("0x11"); // 17
		Number("0b11"); // 3
		Number("0o11"); // 9
		Number("foo"); // NaN
		Number("100a"); // NaN
		Number("-Infinity"); // -Infinity
		
		


# Math
Math is a built-in object that has properties and methods for mathematical constants and functions. It's not a function object.Math works with the Number type. It doesn't work with BigInt.

Unlike many other global objects, Math is not a constructor. All properties and methods of Math are static. You refer to the constant pi as Math.PI and you call the sine function as Math.sin(x), where x is the method's argument. Constants are defined with the full precision of real numbers in JavaScript.


# Examples
Converting between degrees and radians
The trigonometric functions sin(), cos(), tan(), asin(), acos(), atan(), and atan2() expect (and return) angles in radians.

Since humans tend to think in degrees, and some functions (such as CSS transforms) can accept degrees, it is a good idea to keep functions handy that convert between the two:


			function degToRad(degrees) {
			  return degrees * (Math.PI / 180);
			}

			function radToDeg(rad) {
			  return rad / (Math.PI / 180);
			}



#  Primitive and Non-Primitive

Primitive vs Non-Primitive


Before I go into what the two categories of data types are, I will list which data types belong in which category.
Primitive


• Numbers

• Strings

• Booleans

• undefined

• null

Non-Primitive (referred to collectively as Objects)

• Objects

• Arrays

• Functions


 Primitives :

		let a = 5
		let b = a
		console.log(a) // 5
		console.log(b) // 5
		console.log(a === b) // true
		a = 10
		console.log(a) // 10
		console.log(b) // 5
		console.log(a === b) // false
		
		
		
		
Non-Primitives (Objects):

		let a = [10]
		let b = a
		console.log(a === b) // true
		a.push(10)
		console.log(a) // [10, 10]
		console.log(a === b) // true
		
		
		
# DOM
		
		
		DOM bukan bagian dari JavaScript, melainkan browser (Web API)”


# Mengubah Konten Element		
		
-    Element.textContent

Element.textContent dapat kita gunakan untuk mengubah teks di dalam sebuah element

 -  Element.innerHTML

Element.innerHTML dapat kita gunakan untukmengubah konten HTML di dalam sebuah element
		
		
# Menangkap Interaksi User

-   Element.addEventListener(“event”)



-   Element.onevent

		
		
EventListener - Click


Misalkan kita mempunyai element <input id=”user-input” />  dan <button id=”alert-button”>show</button>. 
Kita ingin menampilkan pop up box yang berisi teks di dalam input tadi.


		// cari dulu kedua element tersebut berdasarkan id-nya

		const input = document.getElementById(“user-input”)
		const button = document.getElementById(“alert-button”)

# EventListener - Blur

“Blur”, lawan dari “focus”, adalah event di mana sebuah element kehilangan fokus dari user (misal user klk mouse di luar element tersebut atau user klik tab untuk berpindah element)

Misalkan kita ingin memvalidasi isi dari <input id=”username” /> agar panjangnya minimal 6 karakter..


		// cari dulu element tersebut berdasarkan id-nya

		const input = document.getElementById(“username”)

		// tambahkan event listener
		input.addEventListener(“blur”, () => {
			if(input.value.length < 6) alert(“Panjang username minimal 6”)
		})
		
		
		
# EventListener - Form Submission		
		
	Misalkan kita mempunyai element beberapa input dalam sebuah form <input name=”email /> dan <input type=”password” name=”password” />. Bagaimana caranya  kita mendapatkan isi dari kedua input tersebut saat submit form?

		
Ada 2 cara:

•  Pasang event listener di kedua input dan tombol submit, lalu saat tombol diklik, baca value dari kedua input tersebut. 
•  Pasang event listener di form, lalu gunakan FormData untuk mengambil data dari masing-masing input
		
		
		const form = document.getElementById(“form”)

		form.addEventListener(“submit”, function(event) {
			// cegah page refresh
			event.preventDefault()

			const formData = new FormData(form)
			const values = Object.fromEntries(formData) // { email: ... }
		})



		


		
		
		
		
		
		
