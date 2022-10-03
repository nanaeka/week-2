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





